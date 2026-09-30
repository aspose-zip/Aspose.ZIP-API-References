---
title: "UueArchive.UueArchive"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "UueArchive कंस्ट्रक्टर। एन्कोडिंग के लिए तैयार UueArchive क्लास का नया इंस्टेंस इनिशियलाइज़ करता है"
type: docs
weight: 10
url: /hi/net/aspose.zip.uue/uuearchive/uuearchive/
---
## UueArchive() {#constructor}

एन्कोडिंग के लिए तैयार [`UueArchive`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public UueArchive()
```

## उदाहरण

निम्नलिखित उदाहरण दिखाता है कि फ़ाइल को uuencode कैसे करें।

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.uue");
}
```

### संबंधित देखें

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(Stream) {#constructor_1}

डिकोडिंग के लिए तैयार [`UueArchive`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public UueArchive(Stream sourceStream)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| sourceStream | स्ट्रीम | आर्काइव का स्रोत। |

## टिप्पणियाँ

यह कंस्ट्रक्टर डिकोड नहीं करता। डिकम्प्रेस करने के लिए [`Open`](../open/) मेथड देखें।

## उदाहरण

स्ट्रीम से एक आर्काइव खोलें और उसे `MemoryStream` में एक्सट्रैक्ट करें

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive(File.OpenRead("archive.001")))
  archive.Open().CopyTo(ms);
```

### संबंधित देखें

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(string) {#constructor_2}

[`UueArchive`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public UueArchive(string path)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| पथ | String | आर्काइव फ़ाइल का पथ। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *path* शून्य है। |
| SecurityException | कॉलर के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *path* खाली है, केवल सफ़ेद स्थान शामिल हैं, या इसमें अमान्य अक्षर हैं। |
| UnauthorizedAccessException | *path* फ़ाइल तक पहुँच अस्वीकृत है। |
| PathTooLongException | निर्दिष्ट *path*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 अक्षरों से कम होने चाहिए, और फ़ाइल नाम 260 अक्षरों से कम होने चाहिए। |
| NotSupportedException | *path* पर फ़ाइल में स्ट्रिंग के मध्य में कोलन (:) है। |
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, जैसे कि यह अनमैप्ड ड्राइव पर है। |
| FileNotFoundException | फ़ाइल नहीं मिली। |
| IOException | फ़ाइल पहले से ही खुली है। |

## टिप्पणियाँ

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता। डिकम्प्रेस करने के लिए [`Open`](../open/) मेथड देखें।

## उदाहरण

फ़ाइल से पथ द्वारा एक अभिलेख खोलें और इसे एक `MemoryStream` में डिकोड करें

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive("archive.uue"))
  archive.Open().CopyTo(ms);
```

### संबंधित देखें

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


