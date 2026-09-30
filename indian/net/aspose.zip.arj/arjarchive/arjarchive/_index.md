---
title: "ArjArchive.ArjArchive"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "ArjArchive कंस्ट्रक्टर। ArjArchive क्लास का नया इंस्टेंस इनिशियलाइज़ करता है और एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।"
type: docs
weight: 10
url: /hi/net/aspose.zip.arj/arjarchive/arjarchive/
---
## ArjArchive(Stream, ArjLoadOptions) {#constructor}

[`ArjArchive`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है और एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

```csharp
public ArjArchive(Stream extractionSource, ArjLoadOptions loadOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| extractionSource | स्ट्रीम | आर्काइव का स्रोत। |
| loadOptions | ArjLoadOptions | मौजूदा आर्काइव को लोड करने के विकल्प। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *extractionSource* null है। |
| ArgumentException | &gt;*extractionSource* seeking का समर्थन नहीं करता। |
| InvalidDataException | आर्काइव के लिए गलत सिग्नेचर। - या - फ़ाइल एक ARJ आर्काइव नहीं है। |
| EndOfStreamException | स्ट्रीम के अंत तक पहुँचने से पहले सभी हेडर बाइट्स या नाम बाइट्स पढ़े जाने पर फेंका जाता है। |
| NotSupportedException | आर्काइव खराब है। |

## टिप्पणियाँ

यह कंस्ट्रक्टर किसी भी एंट्री को डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए [`Extract`](../../arjentryplain/extract/) मेथड देखें।

### संबंधित देखें

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)

---

## ArjArchive(string, ArjLoadOptions) {#constructor_1}

[`ArjArchive`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है और एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

```csharp
public ArjArchive(string path, ArjLoadOptions loadOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| पथ | String | आर्काइव फ़ाइल का पथ। |
| loadOptions | ArjLoadOptions | मौजूदा आर्काइव को लोड करने के विकल्प। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *path* शून्य है। |
| SecurityException | कॉलर के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *path* खाली है, केवल सफ़ेद स्थान शामिल हैं, या इसमें अमान्य अक्षर हैं। |
| UnauthorizedAccessException | *path* फ़ाइल तक पहुँच अस्वीकृत है। |
| PathTooLongException | निर्दिष्ट *path*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 अक्षरों से कम होने चाहिए, और फ़ाइल नाम 260 अक्षरों से कम होने चाहिए। |
| NotSupportedException | *path* पर फ़ाइल में स्ट्रिंग के मध्य में कोलन (:) है। |
| FileNotFoundException | फ़ाइल नहीं मिली। |
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, जैसे कि यह अनमैप्ड ड्राइव पर है। |
| IOException | फ़ाइल पहले से ही खुली है। |
| EndOfStreamException | स्ट्रीम के अंत तक पहुँचने से पहले सभी हेडर बाइट्स या नाम बाइट्स पढ़े जाने पर फेंका जाता है। |
| InvalidDataException | ARJ मैजिक नंबर अमान्य है या हेडर आकार सीमा से बाहर है। |

## टिप्पणियाँ

यह कंस्ट्रक्टर किसी भी एंट्री को अनपैक नहीं करता है। डिकम्प्रेस करने के लिए [`Extract`](../../arjentryplain/extract/) मेथड देखें।

## उदाहरण

निम्नलिखित उदाहरण दिखाता है कि सभी एंट्रीज़ को एक डायरेक्टरी में कैसे एक्सट्रैक्ट किया जाए।

```csharp
using (var archive = new ArjArchive("archive.arj")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### संबंधित देखें

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


