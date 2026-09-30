---
title: "LzxArchive.LzxArchive"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "LzxArchive कन्स्ट्रक्टर। LzxArchive क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है"
type: docs
weight: 10
url: /hi/net/aspose.zip.lzx/lzxarchive/lzxarchive/
---
## LzxArchive(Stream, LzxLoadOptions) {#constructor}

[`LzxArchive`](../) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

```csharp
public LzxArchive(Stream extractionSource, LzxLoadOptions loadOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| extractionSource | स्ट्रीम | आर्काइव का स्रोत। |
| loadOptions | LzxLoadOptions | मौजूदा आर्काइव को लोड करने के विकल्प। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *extractionSource* null है। |
| ArgumentException | *extractionSource* सीकिंग का समर्थन नहीं करता है। |
| InvalidDataException | आर्काइव के लिए गलत सिग्नेचर। - या - फ़ाइल एक LZX आर्काइव नहीं है। |
| NotImplementedException | Lzx आर्काइव में मर्ज्ड एंट्रीज़ हैं। |
| EndOfStreamException | *extractionSource* स्ट्रीम बहुत छोटी है। |
| ObjectDisposedException | यदि स्ट्रीम बंद कर दिया गया हो तो थ्रो किया जाता है। |
| IOException | एक I/O त्रुटि हुई। |

## टिप्पणियाँ

यह कन्स्ट्रक्टर किसी भी एंट्री को डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए [`Extract`](../../lzxarchiveentry/extract/) मेथड देखें।

### संबंधित देखें

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzxArchive(string, LzxLoadOptions) {#constructor_1}

[`LzxArchive`](../) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

```csharp
public LzxArchive(string path, LzxLoadOptions loadOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| पथ | String | आर्काइव फ़ाइल का पूर्ण योग्य या सापेक्ष पथ। |
| loadOptions | LzxLoadOptions | मौजूदा आर्काइव को लोड करने के विकल्प। |

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
| NotImplementedException | Lzx आर्काइव में मर्ज्ड एंट्रीज़ हैं। |
| EndOfStreamException | फ़ाइल बहुत छोटी है। |
| ObjectDisposedException | यदि स्ट्रीम बंद कर दिया गया हो तो थ्रो किया जाता है। |

## टिप्पणियाँ

यह कन्स्ट्रक्टर किसी भी एंट्री को डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए [`Extract`](../../lzxarchiveentry/extract/) मेथड देखें।

## उदाहरण

निम्न उदाहरण एक आर्काइव को एक्सट्रैक्ट करता है, फिर पहली एंट्री को `MemoryStream` में डिकम्प्रेस करता है।

```csharp
var extracted = new MemoryStream();
using (LzxArchive archive = new LzxArchive("sample.lzx"))
{
    archive.Entries[0].Extract(extracted);
}
```

### संबंधित देखें

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)


