---
title: GzipArchive.GzipArchive
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: GzipArchive नर्मत. क एक नय उदहरण प्ररंभ करत हैGzipArchive संपड़त करने के लए तैयर वर्ग .
type: docs
weight: 10
url: /hi/net/aspose.zip.gzip/gziparchive/gziparchive/
---
## GzipArchive() {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`GzipArchive`](../) संपीड़ित करने के लिए तैयार वर्ग .

```csharp
public GzipArchive()
```

### उदाहरण

निम्न उदाहरण दिखाता है कि किसी फ़ाइल को कैसे कंप्रेस करना है.

```csharp
using (GzipArchive archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### यह सभी देखें

* class [GzipArchive](../)
* नाम स्थान [Aspose.Zip.Gzip](../../gziparchive/)
* सभा [Aspose.Zip](../../../)

---

## GzipArchive(Stream, bool) {#constructor_1}

का एक नया उदाहरण प्रारंभ करता है[`GzipArchive`](../) डीकंप्रेसिंग के लिए तैयार वर्ग।

```csharp
public GzipArchive(Stream sourceStream, bool parseHeader = false)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | Stream | संग्रह का स्रोत। |
| parseHeader | Boolean | नाम सहित गुणों का पता लगाने के लिए स्ट्रीम हेडर को पार्स करना है या नहीं। खोज योग्य स्ट्रीम के लिए ही समझ में आता है। |

### टिप्पणियों

यह कंस्ट्रक्टर डीकंप्रेस नहीं करता है। देखना[`Open`](../open/) डीकंप्रेसिंग के लिए विधि.

### उदाहरण

एक स्ट्रीम से एक संग्रह खोलें और इसे एक में निकालें`मेमोरीस्ट्रीम`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive(File.OpenRead("archive.gz")))
  archive.Open().CopyTo(ms);
```

### यह सभी देखें

* class [GzipArchive](../)
* नाम स्थान [Aspose.Zip.Gzip](../../gziparchive/)
* सभा [Aspose.Zip](../../../)

---

## GzipArchive(string, bool) {#constructor_2}

का एक नया उदाहरण प्रारंभ करता है[`GzipArchive`](../) वर्ग.

```csharp
public GzipArchive(string path, bool parseHeader = false)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | String | संग्रह फ़ाइल का पथ। |
| parseHeader | Boolean | नाम सहित गुणों का पता लगाने के लिए स्ट्रीम हेडर को पार्स करना है या नहीं। खोज योग्य स्ट्रीम के लिए ही समझ में आता है। |

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

यह कंस्ट्रक्टर डीकंप्रेस नहीं करता है। देखना[`Open`](../open/) डीकंप्रेसिंग के लिए विधि.

### उदाहरण

फ़ाइल से पथ द्वारा एक संग्रह खोलें और इसे एक में निकालें`मेमोरीस्ट्रीम`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive("archive.gz"))
  archive.Open().CopyTo(ms);
```

### यह सभी देखें

* class [GzipArchive](../)
* नाम स्थान [Aspose.Zip.Gzip](../../gziparchive/)
* सभा [Aspose.Zip](../../../)


