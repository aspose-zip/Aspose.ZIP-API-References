---
title: ZArchive.SetSource
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: ZArchive तरक. समग्र क संग्रह के भतर संपड़त करने के लए सेट करत है
type: docs
weight: 50
url: /hi/net/aspose.zip.z/zarchive/setsource/
---
## SetSource(Stream) {#setsource_1}

सामग्री को संग्रह के भीतर संपीड़ित करने के लिए सेट करता है।

```csharp
public void SetSource(Stream source)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| source | Stream | संग्रह के लिए इनपुट स्ट्रीम। |

### उदाहरण

```csharp
using (var archive = new ZArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.Z");
}
```

### यह सभी देखें

* class [ZArchive](../)
* नाम स्थान [Aspose.Zip.Z](../../zarchive/)
* सभा [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

सामग्री को संग्रह के भीतर संपीड़ित करने के लिए सेट करता है।

```csharp
public void SetSource(FileInfo fileInfo)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo जो इनपुट स्ट्रीम के रूप में खोला जाएगा। |

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

### उदाहरण

```csharp
using (var archive = new ZArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bin.Z");
}
```

### यह सभी देखें

* class [ZArchive](../)
* नाम स्थान [Aspose.Zip.Z](../../zarchive/)
* सभा [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

सामग्री को संग्रह के भीतर संपीड़ित करने के लिए सेट करता है।

```csharp
public void SetSource(string sourcePath)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourcePath | String | फ़ाइल का पथ जो इनपुट स्ट्रीम के रूप में खोला जाएगा। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *sourcePath* अशक्त या खाली स्ट्रिंग है। |
| SecurityException | कॉल करने वाले के पास संसाधन तक पहुँचने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *sourcePath* खाली है, केवल सफेद स्थान हैं, या अमान्य वर्ण हैं। |
| UnauthorizedAccessException | फ़ाइल तक पहुंच*sourcePath* वर्जित किया गया है। |
| PathTooLongException | विष्तृत*sourcePath*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 वर्णों से कम होने चाहिए और फ़ाइल नाम 260 वर्णों से कम होने चाहिए। |
| NotSupportedException | पर फाइल करें*sourcePath* स्ट्रिंग के बीच में एक कोलन (:) होता है। |

### उदाहरण

```csharp
using (var archive = new ZArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("data.bin.Z");
}
```

### यह सभी देखें

* class [ZArchive](../)
* नाम स्थान [Aspose.Zip.Z](../../zarchive/)
* सभा [Aspose.Zip](../../../)


