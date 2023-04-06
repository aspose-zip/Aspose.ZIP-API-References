---
title: LzipArchive.LzipArchive
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: LzipArchive नर्मत. क एक नय उदहरण प्ररंभ करत हैLzipArchive .
type: docs
weight: 10
url: /hi/net/aspose.zip.lzip/lziparchive/lziparchive/
---
## LzipArchive(LzipArchiveSettings) {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`LzipArchive`](../) .

```csharp
public LzipArchive(LzipArchiveSettings settings = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| settings | LzipArchiveSettings | शब्दकोश आकार की परिभाषा के साथ विशेष रूप से lzip संग्रह की स्थापना। |

### यह सभी देखें

* class [LzipArchiveSettings](../../lziparchivesettings/)
* class [LzipArchive](../)
* नाम स्थान [Aspose.Zip.Lzip](../../lziparchive/)
* सभा [Aspose.Zip](../../../)

---

## LzipArchive(Stream) {#constructor_1}

का एक नया उदाहरण प्रारंभ करता है[`LzipArchive`](../) डीकंप्रेसिंग के लिए तैयार वर्ग।

```csharp
public LzipArchive(Stream sourceStream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | Stream | संग्रह का स्रोत। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentException | *sourceStream* खोजने योग्य नहीं है। |
| ArgumentNullException | *sourceStream* शून्य है। |
| InvalidDataException | शीर्षलेख lzip प्रकार के संग्रह से मेल नहीं खाते। |

### टिप्पणियों

यह कंस्ट्रक्टर डीकंप्रेस नहीं करता है। देखना[`Extract`](../extract/) डीकंप्रेसिंग के लिए विधि.

### यह सभी देखें

* class [LzipArchive](../)
* नाम स्थान [Aspose.Zip.Lzip](../../lziparchive/)
* सभा [Aspose.Zip](../../../)

---

## LzipArchive(string) {#constructor_2}

का एक नया उदाहरण प्रारंभ करता है[`LzipArchive`](../) डीकंप्रेसिंग के लिए तैयार वर्ग।

```csharp
public LzipArchive(string path)
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
| InvalidDataException | शीर्षलेख lzip प्रकार के संग्रह से मेल नहीं खाते। |

### टिप्पणियों

यह कंस्ट्रक्टर डीकंप्रेस नहीं करता है। देखना[`Extract`](../extract/) डीकंप्रेसिंग के लिए विधि.

### उदाहरण

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzipArchive(sourceLzipFile))
    {
         archive.Extract(extractedFile);
       }
   }
```

### यह सभी देखें

* class [LzipArchive](../)
* नाम स्थान [Aspose.Zip.Lzip](../../lziparchive/)
* सभा [Aspose.Zip](../../../)


