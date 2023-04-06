---
title: ZArchive.ZArchive
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: ZArchive नर्मत. क एक नय उदहरण प्ररंभ करत हैZArchive संपड़त करने के लए तैयर वर्ग .
type: docs
weight: 10
url: /hi/net/aspose.zip.z/zarchive/zarchive/
---
## ZArchive() {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`ZArchive`](../) संपीड़ित करने के लिए तैयार वर्ग .

```csharp
public ZArchive()
```

### यह सभी देखें

* class [ZArchive](../)
* नाम स्थान [Aspose.Zip.Z](../../zarchive/)
* सभा [Aspose.Zip](../../../)

---

## ZArchive(Stream) {#constructor_1}

का एक नया उदाहरण प्रारंभ करता है[`ZArchive`](../) डीकंप्रेसिंग के लिए तैयार वर्ग।

```csharp
public ZArchive(Stream source)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| source | Stream | संग्रह का स्रोत। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentException | *source* खोजने योग्य नहीं है। |
| ArgumentNullException | *source* शून्य है। |

### टिप्पणियों

यह कंस्ट्रक्टर डीकंप्रेस नहीं करता है। देखना[`Extract`](../extract/) डीकंप्रेसिंग के लिए विधि.

### यह सभी देखें

* class [ZArchive](../)
* नाम स्थान [Aspose.Zip.Z](../../zarchive/)
* सभा [Aspose.Zip](../../../)

---

## ZArchive(string) {#constructor_2}

का एक नया उदाहरण प्रारंभ करता है[`ZArchive`](../) डीकंप्रेसिंग के लिए तैयार वर्ग।

```csharp
public ZArchive(string path)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | String | संग्रह के स्रोत का पथ. |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *path* शून्य है। |
| SecurityException | कॉल करने वाले के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *path* खाली है, केवल सफेद स्थान हैं, या अमान्य वर्ण हैं। |
| UnauthorizedAccessException | फ़ाइल तक पहुंच*path* वर्जित किया गया है। |
| PathTooLongException | विष्तृत*path*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 वर्णों से कम होने चाहिए और फ़ाइल नाम 260 वर्णों से कम होने चाहिए। |
| NotSupportedException | पर फाइल करें*path* स्ट्रिंग के बीच में एक कोलन (:) होता है। |

### टिप्पणियों

यह कंस्ट्रक्टर डीकंप्रेस नहीं करता है। देखना[`Extract`](../extract/) डीकंप्रेसिंग के लिए विधि.

### यह सभी देखें

* class [ZArchive](../)
* नाम स्थान [Aspose.Zip.Z](../../zarchive/)
* सभा [Aspose.Zip](../../../)


