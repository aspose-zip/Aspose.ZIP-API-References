---
title: "AppleArchive.AppleArchive"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "AppleArchive कंस्ट्रक्टर। निर्मित एंट्रीज़ के लिए उपयोग की जाने वाली सेटिंग्स के साथ AppleArchive क्लास का नया उदाहरण प्रारंभ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.zip.apple/applearchive/applearchive/
---
## AppleArchive(AppleArchiveEntrySettings) {#constructor}

निर्मित एंट्रीज़ के लिए उपयोग की जाने वाली सेटिंग्स के साथ [`AppleArchive`](../) क्लास का नया उदाहरण प्रारंभ करता है।

```csharp
public AppleArchive(AppleArchiveEntrySettings newEntrySettings = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| newEntrySettings | AppleArchiveEntrySettings | नए Apple Archive को बनाने के दौरान उपयोग की जाने वाली सेटिंग्स। |

### संबंधित देखें

* class [AppleArchiveEntrySettings](../../applearchiveentrysettings/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(Stream, AppleArchiveLoadOptions) {#constructor_1}

[`AppleArchive`](../) क्लास का नया उदाहरण प्रारंभ करता है और अभिलेख से निकाली जा सकने वाली एंट्री सूची बनाता है।

```csharp
public AppleArchive(Stream sourceStream, AppleArchiveLoadOptions loadOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| sourceStream | स्ट्रीम | आर्काइव का स्रोत। |
| loadOptions | AppleArchiveLoadOptions | मौजूदा आर्काइव को लोड करने के विकल्प। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *sourceStream* null है। |
| ArgumentException | *sourceStream* सर्चेबल नहीं है। |
| InvalidDataException | *sourceStream* एक मान्य Apple Archive नहीं है। |
| EndOfStreamException | अभिलेख एंट्रीज़ के पार्सिंग के दौरान स्ट्रीम अप्रत्याशित रूप से समाप्त हो जाता है। |

## टिप्पणियाँ

यह कंस्ट्रक्टर कोई भी एंट्री डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए [`ExtractToDirectory`](../extracttodirectory/) और [`Open`](../../applearchiveentry/open/) मेथड्स देखें।

### संबंधित देखें

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(string, AppleArchiveLoadOptions) {#constructor_2}

[`AppleArchive`](../) क्लास का नया उदाहरण प्रारंभ करता है और अभिलेख से निकाली जा सकने वाली एंट्री सूची बनाता है।

```csharp
public AppleArchive(string path, AppleArchiveLoadOptions loadOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| पथ | String | आर्काइव फ़ाइल का पूर्ण योग्य या सापेक्ष पथ। |
| loadOptions | AppleArchiveLoadOptions | मौजूदा आर्काइव को लोड करने के विकल्प। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *path* शून्य है। |
| FileNotFoundException | फ़ाइल नहीं मिली। |
| InvalidDataException | *path* एक मान्य Apple Archive नहीं है। |
| EndOfStreamException | अभिलेख एंट्रीज़ के पार्सिंग के दौरान स्ट्रीम अप्रत्याशित रूप से समाप्त हो जाता है। |

## टिप्पणियाँ

यह कंस्ट्रक्टर कोई भी एंट्री डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए [`ExtractToDirectory`](../extracttodirectory/) और [`Open`](../../applearchiveentry/open/) मेथड्स देखें।

### संबंधित देखें

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


