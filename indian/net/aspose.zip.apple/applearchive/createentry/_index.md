---
title: "AppleArchive.CreateEntry"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "AppleArchive मेथड। संग्रह के भीतर एक एकल प्रविष्टि बनाता है।"
type: docs
weight: 60
url: /hi/net/aspose.zip.apple/applearchive/createentry/
---
## CreateEntry(string, string, bool) {#createentry_2}

आर्काइव के भीतर एक एकल एंट्री बनाता है।

```csharp
public AppleArchiveEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| पथ | String | संकुचित करने वाली फ़ाइल का पथ। |
| openImmediately | Boolean | सही, यदि फ़ाइल को तुरंत खोला जाए, अन्यथा संग्रह सहेजते समय फ़ाइल को खोला जाएगा। |

### रिटर्न वैल्यू

Apple Archive प्रविष्टि इंस्टेंस।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ObjectDisposedException | संग्रह को नष्ट कर दिया गया है। |
| ArgumentException | *name* खाली है। |
| ArgumentNullException | *path* `null` है। |

### संबंधित देखें

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

आर्काइव के भीतर एक एकल एंट्री बनाता है।

```csharp
public AppleArchiveEntry CreateEntry(string name, Stream source)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| स्रोत | स्ट्रीम | प्रविष्टि के लिए इनपुट स्ट्रीम। |

### रिटर्न वैल्यू

Apple Archive प्रविष्टि इंस्टेंस।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ObjectDisposedException | संग्रह को नष्ट कर दिया गया है। |
| ArgumentException | *name* खाली है। |
| ArgumentNullException | *source* `null` है। |

### संबंधित देखें

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

आर्काइव के भीतर एक एकल एंट्री बनाता है।

```csharp
public AppleArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| fileInfo | FileInfo | संकुचित की जाने वाली फ़ाइल का मेटाडाटा। |
| openImmediately | Boolean | सही, यदि फ़ाइल को तुरंत खोला जाए, अन्यथा संग्रह सहेजते समय फ़ाइल को खोला जाएगा। |

### रिटर्न वैल्यू

Apple Archive प्रविष्टि इंस्टेंस।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ObjectDisposedException | संग्रह को नष्ट कर दिया गया है। |
| ArgumentException | *name* खाली है। |
| ArgumentNullException | *fileInfo* `null` है। |

### संबंधित देखें

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


