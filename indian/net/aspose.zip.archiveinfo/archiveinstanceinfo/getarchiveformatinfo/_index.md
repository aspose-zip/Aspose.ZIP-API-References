---
title: ArchiveInstanceInfo.GetArchiveFormatInfo
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: ArchiveInstanceInfo तरक. संग्रह प्ररूप जनकर प्रप्त करत है
type: docs
weight: 50
url: /hi/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveformatinfo/
---
## GetArchiveFormatInfo(string) {#getarchiveformatinfo_1}

संग्रह प्रारूप जानकारी प्राप्त करता है।

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(string fileName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | String | संग्रह फ़ाइल का फ़ाइल नाम। |

### प्रतिलाभ की मात्रा

संग्रह प्रारूप के बारे में जानकारी या यदि प्रारूप का पता नहीं चला तो अशक्त।

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *fileName* शून्य है। |
| SecurityException | कॉल करने वाले के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *fileName* खाली है, केवल सफेद स्थान हैं, या अमान्य वर्ण हैं। |
| UnauthorizedAccessException | फ़ाइल तक पहुंच*fileName* वर्जित किया गया है। |
| PathTooLongException | विष्तृत*fileName* सिस्टम-परिभाषित अधिकतम लंबाई से अधिक है। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 वर्णों से कम होने चाहिए और फ़ाइल नाम 260 वर्णों से कम होने चाहिए। |
| NotSupportedException | पर फाइल करें*fileName* स्ट्रिंग के बीच में एक कोलन (:) होता है। |
| IOException | फ़ाइल खोलते समय I/O त्रुटि हुई। |

### यह सभी देखें

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* नाम स्थान [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* सभा [Aspose.Zip](../../../)

---

## GetArchiveFormatInfo(Stream) {#getarchiveformatinfo}

संग्रह प्रारूप जानकारी प्राप्त करता है।

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(Stream stream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | Stream | संग्रह फ़ाइल की धारा। |

### प्रतिलाभ की मात्रा

संग्रह प्रारूप के बारे में जानकारी या यदि प्रारूप का पता नहीं चला तो अशक्त।

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *stream* शून्य है। |
| ArgumentException | *stream* खोजने योग्य नहीं है। |

### यह सभी देखें

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* नाम स्थान [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* सभा [Aspose.Zip](../../../)


