---
title: "LhaArchive.LhaArchive"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "LhaArchive कंस्ट्रक्टर। LhaArchive क्लास का नया इंस्टेंस इनिशियलाइज़ करता है और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है"
type: docs
weight: 10
url: /hi/net/aspose.zip.lha/lhaarchive/lhaarchive/
---
## LhaArchive(Stream, LhaLoadOptions) {#constructor}

एक नया इंस्टेंस इनिशियलाइज़ करता है [`LhaArchive`](../) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

```csharp
public LhaArchive(Stream sourceStream, LhaLoadOptions loadOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| sourceStream | स्ट्रीम | आर्काइव का स्रोत। |
| loadOptions | LhaLoadOptions | मौजूदा आर्काइव को लोड करने के विकल्प। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *sourceStream* null है |
| ArgumentException | *sourceStream* अनसीकएबल है। |
| InvalidDataException | अअनुचित डेटा मिला। |
| EndOfStreamException | जब स्ट्रीम का अंत पहुँच जाता है और अपेक्षित बाइट्स की संख्या पढ़ी नहीं जाती, तो यह अपवाद फेंका जाता है। |
| ObjectDisposedException | जब ऑब्जेक्ट को डिस्पोज़ किया गया हो तब थ्रो किया जाता है। |

## टिप्पणियाँ

यह कंस्ट्रक्टर किसी एंट्री को डिकम्प्रेस नहीं करता। डिकम्प्रेस करने के लिए [`Extract`](../../lhaarchiveentry/extract/) मेथड देखें।

### संबंधित देखें

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LhaArchive(string, LhaLoadOptions) {#constructor_1}

एक नया इंस्टेंस इनिशियलाइज़ करता है [`LhaArchive`](../) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

```csharp
public LhaArchive(string path, LhaLoadOptions loadOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| पथ | String | आर्काइव फ़ाइल का पूर्ण योग्य या सापेक्ष पथ। |
| loadOptions | LhaLoadOptions | मौजूदा आर्काइव को लोड करने के विकल्प। |

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
| InvalidDataException | फ़ाइल भ्रष्ट है। |
| EndOfStreamException | जब स्ट्रीम का अंत पहुँच जाता है और अपेक्षित बाइट्स की संख्या पढ़ी नहीं जाती, तो यह अपवाद फेंका जाता है। |
| ObjectDisposedException | जब ऑब्जेक्ट को डिस्पोज़ किया गया हो तब थ्रो किया जाता है। |

## टिप्पणियाँ

यह कंस्ट्रक्टर किसी एंट्री को डिकम्प्रेस नहीं करता। डिकम्प्रेस करने के लिए [`Extract`](../../lhaarchiveentry/extract/) मेथड देखें।

## उदाहरण

निम्न उदाहरण एक आर्काइव को एक्सट्रैक्ट करता है, फिर पहली एंट्री को `MemoryStream` में डिकम्प्रेस करता है।

```csharp
var extracted = new MemoryStream();
using (LhaArchive archive = new LhaArchive("sample.lzh"))
{
    archive.Entries[0].Extract(extracted);
}
```

### संबंधित देखें

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)


