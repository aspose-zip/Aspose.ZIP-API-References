---
title: "GetFormatInfo"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: 
type: docs
weight: 20
url: /hi/net/aspose.zip.archiveinfo/archiveformatdetector/getformatinfo/
---
## ArchiveFormatDetector.GetFormatInfo method (1 of 2)

फ़ॉर्मेट जानकारी प्राप्त करता है।

```csharp
public ArchiveFormatInfo GetFormatInfo(string fileName)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| fileName | String | आर्काइव फ़ाइल का फ़ाइलनाम। |

### रिटर्न वैल्यू

आर्काइव फ़ॉर्मेट के बारे में जानकारी या यदि फ़ॉर्मेट का पता नहीं चला तो null।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *fileName* null है। |
| SecurityException | कॉलर के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *fileName* खाली है, केवल व्हाइट स्पेस शामिल है, या अवैध अक्षर शामिल हैं। |
| UnauthorizedAccessException | फ़ाइल *fileName* तक पहुँच अस्वीकृत है। |
| PathTooLongException | निर्दिष्ट *fileName* सिस्टम-परिभाषित अधिकतम लंबाई से अधिक है। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पाथ 248 अक्षरों से कम होना चाहिए, और फ़ाइल नाम 260 अक्षरों से कम होना चाहिए। |
| NotSupportedException | *fileName* पर फ़ाइल में स्ट्रिंग के मध्य में कोलन (:) है। |
| IOException | फ़ाइल खोलते समय एक I/O त्रुटि हुई। |

### संबंधित देखें

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

---

## ArchiveFormatDetector.GetFormatInfo method (2 of 2)

फ़ॉर्मेट जानकारी प्राप्त करता है।

```csharp
public ArchiveFormatInfo GetFormatInfo(Stream stream)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| स्ट्रीम | स्ट्रीम | आर्काइव फ़ाइल की स्ट्रीम। |

### रिटर्न वैल्यू

आर्काइव फ़ॉर्मेट के बारे में जानकारी या यदि फ़ॉर्मेट का पता नहीं चला तो null।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *stream* शून्य है। |
| ArgumentException | *stream* seekable नहीं है। |

### संबंधित देखें

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

<!-- संपादित न करें: xmldocmd द्वारा Aspose.Zip.dll के लिए उत्पन्न किया गया -->
