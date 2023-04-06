---
title: SevenZipArchiveEntry.Extract
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: SevenZipArchiveEntry तरक. दए गए पथ द्वर फइल सस्टम में प्रवेश क नकलत है
type: docs
weight: 80
url: /hi/net/aspose.zip.sevenzip/sevenziparchiveentry/extract/
---
## Extract(string, string) {#extract}

दिए गए पथ द्वारा फाइल सिस्टम में प्रवेश को निकालता है।

```csharp
public FileInfo Extract(string path, string password = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | String | गंतव्य फ़ाइल का पथ। यदि फ़ाइल पहले से मौजूद है, तो इसे अधिलेखित कर दिया जाएगा। |
| password | String | डिक्रिप्शन के लिए वैकल्पिक पासवर्ड। |

### प्रतिलाभ की मात्रा

रचित फ़ाइल की फ़ाइल जानकारी।

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *path* शून्य है। |
| SecurityException | कॉल करने वाले के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *path* खाली है, केवल सफेद स्थान हैं, या अमान्य वर्ण हैं। |
| UnauthorizedAccessException | फ़ाइल तक पहुंच*path* वर्जित किया गया है। |
| PathTooLongException | विष्तृत*path*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 वर्णों से कम होने चाहिए और फ़ाइल नाम 260 वर्णों से कम होने चाहिए। |
| NotSupportedException | पर फाइल करें*path* स्ट्रिंग के बीच में एक कोलन (:) होता है। |

### उदाहरण

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### यह सभी देखें

* class [SevenZipArchiveEntry](../)
* नाम स्थान [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* सभा [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

प्रदान की गई स्ट्रीम की प्रविष्टि निकालता है.

```csharp
public void Extract(Stream destination, string password = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destination | Stream | गंतव्य धारा। लिखने योग्य होना चाहिए। |
| password | String | डिक्रिप्शन के लिए वैकल्पिक पासवर्ड। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentException | *destination* लिखने का समर्थन नहीं करता। |
| InvalidOperationException | संग्रह निष्कर्षण के लिए नहीं खोला गया है। - या - यह प्रविष्टि एक निर्देशिका है। |
| InvalidDataException | प्रविष्टि में गलत डेटा। |

### उदाहरण

पासवर्ड के साथ ज़िप आर्काइव की एक प्रविष्टि निकालें।

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### यह सभी देखें

* class [SevenZipArchiveEntry](../)
* नाम स्थान [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* सभा [Aspose.Zip](../../../)


