---
title: ZArchive.Extract
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: ZArchive तरक. Z संग्रह क एक स्ट्रम में नकलत है
type: docs
weight: 30
url: /hi/net/aspose.zip.z/zarchive/extract/
---
## Extract(Stream) {#extract_2}

Z संग्रह को एक स्ट्रीम में निकालता है।

```csharp
public void Extract(Stream destination)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destination | Stream | विघटित डेटा को संग्रहीत करने के लिए स्ट्रीम करें। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| InvalidDataException | डेटा को डिकम्प्रेस नहीं किया जा सकता है। |

### उदाहरण

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new ZArchive(zFile))
        {
            archive.Extract(extractedFile);
        }
    }
}
```

### यह सभी देखें

* class [ZArchive](../)
* नाम स्थान [Aspose.Zip.Z](../../zarchive/)
* सभा [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Z संग्रह को एक फ़ाइल में निकालता है।

```csharp
public void Extract(FileInfo fileInfo)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo विघटित डेटा संग्रहीत करने के लिए। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| SecurityException | कॉलर के पास खोलने के लिए आवश्यक अनुमति नहीं है*fileInfo*. |
| ArgumentException | फ़ाइल पथ खाली है या केवल सफेद स्थान हैं। |
| FileNotFoundException | फ़ाइल नहीं मिली. |
| UnauthorizedAccessException | फ़ाइल का पथ केवल पढ़ने के लिए है या एक निर्देशिका है। |
| ArgumentNullException | *fileInfo* शून्य है। |
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, जैसे कि मैप न की गई ड्राइव पर होना। |
| IOException | फाइल पहले से ही खुली हुई है। |
| InvalidDataException | डेटा को डिकम्प्रेस नहीं किया जा सकता है। |

### उदाहरण

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ZArchive(zFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### यह सभी देखें

* class [ZArchive](../)
* नाम स्थान [Aspose.Zip.Z](../../zarchive/)
* सभा [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Z आर्काइव को फ़ाइल में पाथ के अनुसार निकालता है.

```csharp
public FileInfo Extract(string path)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | String | फ़ाइल का पथ जो विघटित डेटा को संग्रहीत करेगा। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *path* शून्य है। |
| SecurityException | कॉल करने वाले के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *path* खाली है, केवल सफेद स्थान हैं, या अमान्य वर्ण हैं। |
| UnauthorizedAccessException | फ़ाइल तक पहुंच*path* वर्जित किया गया है। |
| PathTooLongException | विष्तृत*path*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 वर्णों से कम होने चाहिए और फ़ाइल नाम 260 वर्णों से कम होने चाहिए। |
| NotSupportedException | पर फाइल करें*path* स्ट्रिंग के बीच में एक कोलन (:) होता है। |
| InvalidDataException | डेटा को डिकम्प्रेस नहीं किया जा सकता है। |

### उदाहरण

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ZArchive(zFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### यह सभी देखें

* class [ZArchive](../)
* नाम स्थान [Aspose.Zip.Z](../../zarchive/)
* सभा [Aspose.Zip](../../../)


