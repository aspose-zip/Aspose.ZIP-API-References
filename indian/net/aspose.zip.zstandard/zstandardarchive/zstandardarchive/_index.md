---
title: "ZstandardArchive.ZstandardArchive"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "ZstandardArchive कंस्ट्रक्टर। संपीड़न के लिए तैयार ZstandardArchive क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है"
type: docs
weight: 10
url: /hi/net/aspose.zip.zstandard/zstandardarchive/zstandardarchive/
---
## ZstandardArchive() {#constructor}

संपीड़न के लिए तैयार [`ZstandardArchive`](../) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public ZstandardArchive()
```

## उदाहरण

निम्नलिखित उदाहरण दिखाता है कि फ़ाइल को कैसे संपीड़ित किया जाए।

```csharp
using (ZstandardArchive archive = new ZstandardArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.zst");
}
```

### संबंधित देखें

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(Stream, ZstandardLoadOptions) {#constructor_1}

डिकम्प्रेसिंग के लिए तैयार [`ZstandardArchive`](../) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public ZstandardArchive(Stream sourceStream, ZstandardLoadOptions options = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| sourceStream | स्ट्रीम | आर्काइव का स्रोत। |
| विकल्प | ZstandardLoadOptions | आर्काइव लोड करने के विकल्प। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ObjectDisposedException | यदि स्रोत स्ट्रीम को नष्ट कर दिया गया हो तो यह थ्रो किया जाता है। |
| EndOfStreamException | जब स्ट्रीम का अंत अप्रत्याशित रूप से पहुँच जाता है तो यह थ्रो किया जाता है। |
| IOException | एक I/O त्रुटि हुई। |
| InvalidDataException | जब डेटा अमान्य या भ्रष्ट हो तो फेंका जाता है। |

## टिप्पणियाँ

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता। डिकम्प्रेस करने के लिए [`Open`](../open/) मेथड देखें।

## उदाहरण

स्ट्रीम से एक आर्काइव खोलें और उसे `MemoryStream` में एक्सट्रैक्ट करें

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new ZstandardArchive(File.OpenRead("archive.zst")))
  archive.Open().CopyTo(ms);
```

### संबंधित देखें

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(string, ZstandardLoadOptions) {#constructor_2}

[`ZstandardArchive`](../) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public ZstandardArchive(string path, ZstandardLoadOptions options = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| पथ | String | आर्काइव फ़ाइल का पथ। |
| विकल्प | ZstandardLoadOptions | आर्काइव लोड करने के विकल्प। |

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
| EndOfStreamException | जब स्ट्रीम का अंत अप्रत्याशित रूप से पहुँच जाता है तो यह थ्रो किया जाता है। |
| FileNotFoundException | फ़ाइल नहीं मिली। |
| IOException | फ़ाइल पहले से ही खुली है। |
| InvalidDataException | जब डेटा अमान्य या भ्रष्ट हो तो फेंका जाता है। |

## टिप्पणियाँ

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता। डिकम्प्रेस करने के लिए [`Open`](../open/) मेथड देखें।

## उदाहरण

फ़ाइल पथ से एक आर्काइव खोलें और उसे `MemoryStream` में निकालें

```csharp
var ms = new MemoryStream();
using (ZstandardArchive archive = new ZstandardArchive("archive.zst"))
  archive.Open().CopyTo(ms);
```

### संबंधित देखें

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


