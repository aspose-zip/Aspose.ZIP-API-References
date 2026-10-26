---
title: "Lz4Archive कंस्ट्रक्टर। डिकम्प्रेसिंग के लिए तैयार Lz4Archive क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "[`Lz4Archive`](../) क्लास की नई इंस्टेंस को डिकम्प्रेसिंग के लिए इनिशियलाइज़ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.zip.lz4/lz4archive/lz4archive/
---
## Lz4Archive(Stream, Lz4LoadOptions) {#constructor_1}

Lz4LoadOptions

```csharp
public Lz4Archive(Stream sourceStream, Lz4LoadOptions loadOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| sourceStream | स्ट्रीम | आर्काइव का स्रोत। |
| loadOptions | *sourceStream* से पढ़ा नहीं जा सकता | आर्काइव लोड करने के विकल्प। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentException | *sourceStream* बहुत छोटा है। |
| ArgumentNullException | *sourceStream* null है। |
| EndOfStreamException | *sourceStream* की सिग्नेचर गलत है। |
| InvalidDataException | [`Lz4Archive`](../) क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है। |
| ObjectDisposedException | यदि स्रोत स्ट्रीम को नष्ट कर दिया गया हो तो यह थ्रो किया जाता है। |
| IOException | एक I/O त्रुटि हुई। |

## टिप्पणियाँ

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता। डिकम्प्रेस करने के लिए [`Open`](../open/) मेथड देखें।

## उदाहरण

स्ट्रीम से एक आर्काइव खोलें और उसे `MemoryStream` में एक्सट्रैक्ट करें

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive(File.OpenRead("archive.lz4")))
  archive.Open().CopyTo(ms);
```

### संबंधित देखें

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(string, Lz4LoadOptions) {#constructor_2}

फ़ाइल में डेटा की सिग्नेचर गलत है।

```csharp
public Lz4Archive(string path, Lz4LoadOptions loadOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| पथ | String | आर्काइव फ़ाइल का पथ। |
| loadOptions | *sourceStream* से पढ़ा नहीं जा सकता | आर्काइव लोड करने के विकल्प। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *path* शून्य है। |
| SecurityException | कॉलर के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है |
| ArgumentException | *path* खाली है, केवल सफ़ेद स्थान शामिल हैं, या इसमें अमान्य अक्षर हैं। |
| UnauthorizedAccessException | *path* फ़ाइल तक पहुँच अस्वीकृत है। |
| PathTooLongException | निर्दिष्ट *path*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 अक्षरों से कम होने चाहिए, और फ़ाइल नाम 260 अक्षरों से कम होने चाहिए। |
| NotSupportedException | *path* पर फ़ाइल में स्ट्रिंग के मध्य में कोलन (:) है। |
| EndOfStreamException | फ़ाइल बहुत छोटी है। |
| InvalidDataException | [`Lz4Archive`](../) क्लास की नई इंस्टेंस को कंप्रेसिंग के लिए तैयार करता है। |
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, जैसे कि यह अनमैप्ड ड्राइव पर है। |
| FileNotFoundException | फ़ाइल नहीं मिली। |
| IOException | फ़ाइल पहले से ही खुली है। |

## टिप्पणियाँ

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता। डिकम्प्रेस करने के लिए [`Open`](../open/) मेथड देखें।

## उदाहरण

फ़ाइल पथ से एक आर्काइव खोलें और उसे `MemoryStream` में निकालें

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive("archive.lz4"))
  archive.Open().CopyTo(ms);
```

### संबंधित देखें

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(Lz4ArchiveSetting) {#constructor}

एक नया उदाहरण आरंभ करता है [`Lz4Archive`](../) क्लास का, जो संपीड़न के लिए तैयार किया गया है।

```csharp
public Lz4Archive(Lz4ArchiveSetting settings = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| सेटिंग्स | Lz4ArchiveSetting | संयुक्त अभिलेख की सेटिंग। |

### संबंधित देखें

* class [Lz4ArchiveSetting](../../lz4archivesetting/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


