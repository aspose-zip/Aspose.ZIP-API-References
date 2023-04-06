---
title: LzipArchive.Extract
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: LzipArchive तरक. lzip संग्रह क स्ट्रम में नकलत है.
type: docs
weight: 40
url: /hi/net/aspose.zip.lzip/lziparchive/extract/
---
## Extract(Stream) {#extract_1}

lzip संग्रह को स्ट्रीम में निकालता है.

```csharp
public void Extract(Stream destination)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destination | Stream | विघटित डेटा को संग्रहीत करने के लिए स्ट्रीम करें। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| InvalidOperationException | संग्रह शीर्षलेख और सेवा जानकारी नहीं पढ़ी गई थी। |
| InvalidDataException | हेडर या चेकसम में डेटा में त्रुटि। |
| ArgumentNullException | गंतव्य स्ट्रीम शून्य है। |
| ArgumentException | गंतव्य धारा लेखन का समर्थन नहीं करती है। |

### उदाहरण

```csharp
using (FileStream sourceLzipFile = File.Open(sourceFileName, FileMode.Open))
{
   using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new LzipArchive(sourceLzipFile))
        {
               archive.Extract(extractedFile);
           }
       }
}
```

### यह सभी देखें

* class [LzipArchive](../)
* नाम स्थान [Aspose.Zip.Lzip](../../lziparchive/)
* सभा [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract}

lzip संग्रह को फ़ाइल में निकालता है.

```csharp
public void Extract(FileInfo fileInfo)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo विघटित डेटा संग्रहीत करने के लिए। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| InvalidOperationException | संग्रह शीर्षलेख और सेवा जानकारी नहीं पढ़ी गई थी। |
| SecurityException | कॉलर के पास खोलने के लिए आवश्यक अनुमति नहीं है*fileInfo*. |
| ArgumentException | फ़ाइल पथ खाली है या केवल सफेद स्थान हैं। |
| FileNotFoundException | फ़ाइल नहीं मिली. |
| UnauthorizedAccessException | फ़ाइल का पथ केवल पढ़ने के लिए है या एक निर्देशिका है। |
| ArgumentNullException | *fileInfo* शून्य है। |
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, जैसे कि मैप न की गई ड्राइव पर होना। |
| IOException | फाइल पहले से ही खुली हुई है। |

### उदाहरण

```csharp
using (FileStream lzipFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzipArchive(lzipFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### यह सभी देखें

* class [LzipArchive](../)
* नाम स्थान [Aspose.Zip.Lzip](../../lziparchive/)
* सभा [Aspose.Zip](../../../)

---

## Extract(string) {#extract_2}

lzip आर्काइव को पथ के अनुसार फ़ाइल से निकालता है.

```csharp
public void Extract(string path)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | String | फ़ाइल का पथ जो विघटित डेटा को संग्रहीत करेगा। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| InvalidOperationException | संग्रह शीर्षलेख और सेवा जानकारी नहीं पढ़ी गई थी। |
| ArgumentNullException | *path* शून्य है। |
| SecurityException | कॉल करने वाले के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *path* खाली है, केवल सफेद स्थान हैं, या अमान्य वर्ण हैं। |
| UnauthorizedAccessException | फ़ाइल तक पहुंच*path* वर्जित किया गया है। |
| PathTooLongException | विष्तृत*path*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 वर्णों से कम होने चाहिए और फ़ाइल नाम 260 वर्णों से कम होने चाहिए। |
| NotSupportedException | पर फाइल करें*path* स्ट्रिंग के बीच में एक कोलन (:) होता है। |

### उदाहरण

```csharp
using (FileStream lzipFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzipArchive(xzFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### यह सभी देखें

* class [LzipArchive](../)
* नाम स्थान [Aspose.Zip.Lzip](../../lziparchive/)
* सभा [Aspose.Zip](../../../)


