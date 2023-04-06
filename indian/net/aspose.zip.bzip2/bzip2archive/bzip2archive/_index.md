---
title: Bzip2Archive.Bzip2Archive
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Bzip2Archive नर्मत. क एक नय उदहरण प्ररंभ करत हैBzip2Archive संपड़त करने के लए तैयर वर्ग .
type: docs
weight: 10
url: /hi/net/aspose.zip.bzip2/bzip2archive/bzip2archive/
---
## Bzip2Archive() {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`Bzip2Archive`](../) संपीड़ित करने के लिए तैयार वर्ग .

```csharp
public Bzip2Archive()
```

### उदाहरण

निम्न उदाहरण दिखाता है कि किसी फ़ाइल को कैसे कंप्रेस करना है.

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### यह सभी देखें

* class [Bzip2Archive](../)
* नाम स्थान [Aspose.Zip.Bzip2](../../bzip2archive/)
* सभा [Aspose.Zip](../../../)

---

## Bzip2Archive(Stream) {#constructor_1}

का एक नया उदाहरण प्रारंभ करता है[`Bzip2Archive`](../) डीकंप्रेसिंग के लिए तैयार वर्ग।

```csharp
public Bzip2Archive(Stream sourceStream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | Stream | संग्रह का स्रोत। |

### टिप्पणियों

यह कंस्ट्रक्टर डीकंप्रेस नहीं करता है। देखना[`Open`](../open/) डीकंप्रेसिंग के लिए विधि.

### उदाहरण

एक स्ट्रीम से एक संग्रह खोलें और इसे एक में निकालें`मेमोरीस्ट्रीम`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive(File.OpenRead("archive.bz2")))
  archive.Open().CopyTo(ms);
```

### यह सभी देखें

* class [Bzip2Archive](../)
* नाम स्थान [Aspose.Zip.Bzip2](../../bzip2archive/)
* सभा [Aspose.Zip](../../../)

---

## Bzip2Archive(string) {#constructor_2}

का एक नया उदाहरण प्रारंभ करता है[`Bzip2Archive`](../) डीकंप्रेसिंग के लिए तैयार वर्ग।

```csharp
public Bzip2Archive(string path)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | String | संग्रह फ़ाइल का पथ। |

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
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
  archive.Open().CopyTo(ms);
```

### यह सभी देखें

* class [Bzip2Archive](../)
* नाम स्थान [Aspose.Zip.Bzip2](../../bzip2archive/)
* सभा [Aspose.Zip](../../../)


