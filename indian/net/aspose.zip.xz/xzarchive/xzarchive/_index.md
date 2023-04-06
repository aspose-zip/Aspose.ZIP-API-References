---
title: XzArchive.XzArchive
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: XzArchive नर्मत. क एक नय उदहरण प्ररंभ करत हैXzArchive वर्ग और xz प्ररूप में संग्रह क रचन करत है
type: docs
weight: 10
url: /hi/net/aspose.zip.xz/xzarchive/xzarchive/
---
## XzArchive(XzArchiveSettings) {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`XzArchive`](../) वर्ग और xz प्रारूप में संग्रह की रचना करता है।

```csharp
public XzArchive(XzArchiveSettings settings = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| settings | XzArchiveSettings | विशेष xz संग्रह सेटिंग का सेट: शब्दकोश आकार, ब्लॉक आकार, चेक प्रकार। |

### यह सभी देखें

* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [XzArchive](../)
* नाम स्थान [Aspose.Zip.Xz](../../xzarchive/)
* सभा [Aspose.Zip](../../../)

---

## XzArchive(Stream) {#constructor_1}

का एक नया उदाहरण प्रारंभ करता है[`XzArchive`](../) डीकंप्रेसिंग के लिए तैयार वर्ग।

```csharp
public XzArchive(Stream source)
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

* class [XzArchive](../)
* नाम स्थान [Aspose.Zip.Xz](../../xzarchive/)
* सभा [Aspose.Zip](../../../)

---

## XzArchive(string) {#constructor_2}

का एक नया उदाहरण प्रारंभ करता है[`XzArchive`](../) डीकंप्रेसिंग के लिए तैयार वर्ग।

```csharp
public XzArchive(string path)
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

* class [XzArchive](../)
* नाम स्थान [Aspose.Zip.Xz](../../xzarchive/)
* सभा [Aspose.Zip](../../../)


