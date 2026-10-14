---
title: "IsoArchive.CreateEntry"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "IsoArchive मेथड। ISO इमेज में फ़ाइल जोड़ता है"
type: docs
weight: 40
url: /hi/net/aspose.zip.iso/isoarchive/createentry/
---
## CreateEntry(string, string) {#createentry_2}

ISO इमेज में एक फ़ाइल जोड़ता है।

```csharp
public IsoEntry CreateEntry(string name, string filePath)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| name | String | ISO में फ़ाइल का पथ। |
| filePath | String | फ़ाइल का पथ। |

### रिटर्न वैल्यू

ISO एंट्री निर्मित।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *filePath* शून्य है। |
| ArgumentException | *filePath* खाली है, केवल सफ़ेद स्थान शामिल हैं, या इसमें अमान्य अक्षर हैं। |
| UnauthorizedAccessException | *filePath* फ़ाइल तक पहुँच अस्वीकृत है। |
| PathTooLongException | निर्दिष्ट *filePath* सिस्टम-परिभाषित अधिकतम लंबाई से अधिक है। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 अक्षरों से कम होने चाहिए, और फ़ाइल नाम 260 अक्षरों से कम होने चाहिए। |
| NotSupportedException | *filePath* पर फ़ाइल में स्ट्रिंग के मध्य में कोलन (:) है। |
| IOException | फ़ाइल खोलते समय एक I/O त्रुटि हुई। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, (उदाहरण के लिए, यह अनमैप्ड ड्राइव पर है)। |
| FileNotFoundException | फ़ाइल *filePath* में निर्दिष्ट नहीं मिली। |
| InvalidOperationException | आर्काइव संपादन मोड में नहीं है। |

### संबंधित देखें

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

ISO इमेज में एक फ़ाइल जोड़ता है।

```csharp
public IsoEntry CreateEntry(string name, Stream source)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| name | String | ISO में फ़ाइल का पथ। |
| स्रोत | स्ट्रीम | फ़ाइल डेटा युक्त स्ट्रीम। |

### रिटर्न वैल्यू

ISO एंट्री निर्मित।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| ArgumentNullException | जब *name* या *source* शून्य हो तो फेंका जाता है। |
| InvalidOperationException | आर्काइव संपादन मोड में नहीं है। |

### संबंधित देखें

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string) {#createentry}

ISO इमेज में एक फ़ाइल जोड़ता है।

```csharp
public IsoEntry CreateEntry(string name)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| name | String | ISO में डायरेक्टरी का पाथ। |

### रिटर्न वैल्यू

ISO एंट्री निर्मित।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | `name` null या खाली है। |
| InvalidOperationException | आर्काइव निष्कर्षण के लिए खोला गया है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |

### संबंधित देखें

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


