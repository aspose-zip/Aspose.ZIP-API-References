---
title: "EggArchive.EggArchive"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "EggArchive कंस्ट्रक्टर। स्ट्रीम से EggArchive क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है"
type: docs
weight: 10
url: /hi/net/aspose.zip.egg/eggarchive/eggarchive/
---
## EggArchive(Stream, EggArchiveLoadOptions) {#constructor}

स्ट्रीम से [`EggArchive`](../) क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है।

```csharp
public EggArchive(Stream stream, EggArchiveLoadOptions loadOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| स्ट्रीम | स्ट्रीम | EGG आर्काइव स्ट्रीम। स्ट्रीम को पढ़ने और सीकिंग का समर्थन करना चाहिए। |
| loadOptions | EggArchiveLoadOptions | आर्काइव को लोड करने के विकल्प। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *stream* शून्य है। |
| ArgumentException | *stream* पढ़ने योग्य और खोज योग्य नहीं है। |

### संबंधित देखें

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)

---

## EggArchive(string, EggArchiveLoadOptions) {#constructor_1}

फ़ाइल पथ से [`EggArchive`](../) क्लास का नया उदाहरण प्रारंभ करता है।

```csharp
public EggArchive(string path, EggArchiveLoadOptions loadOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| पथ | String | EGG अभिलेख फ़ाइल का पथ। |
| loadOptions | EggArchiveLoadOptions | आर्काइव को लोड करने के विकल्प। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *path* शून्य है। |
| FileNotFoundException | फ़ाइल मौजूद नहीं है। |
| SecurityException | कॉलर के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *path* खाली है, केवल सफ़ेद स्थान शामिल हैं, या इसमें अमान्य अक्षर हैं। |
| UnauthorizedAccessException | *path* फ़ाइल तक पहुँच अस्वीकृत है। |
| PathTooLongException | निर्दिष्ट *path*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 अक्षरों से कम होने चाहिए, और फ़ाइल नाम 260 अक्षरों से कम होने चाहिए। |
| NotSupportedException | *path* पर फ़ाइल में स्ट्रिंग के मध्य में कोलन (:) है। |
| FileNotFoundException | फ़ाइल नहीं मिली। |
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, जैसे कि यह अनमैप्ड ड्राइव पर है। |
| IOException | फ़ाइल पहले से ही खुली है। |

### संबंधित देखें

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)


