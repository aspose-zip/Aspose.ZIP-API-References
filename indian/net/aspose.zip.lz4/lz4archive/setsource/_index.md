---
title: "Lz4Archive.SetSource"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "Lz4Archive मेथड। आर्काइव के भीतर संकुचित की जाने वाली सामग्री सेट करता है।"
type: docs
weight: 70
url: /hi/net/aspose.zip.lz4/lz4archive/setsource/
---
## SetSource(Stream) {#setsource_2}

आर्काइव के भीतर संपीड़ित की जाने वाली सामग्री को सेट करता है।

```csharp
public void SetSource(Stream source)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| स्रोत | स्ट्रीम | आर्काइव के लिए इनपुट स्ट्रीम। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| InvalidOperationException | आर्काइव को एक्सट्रैक्शन के लिए तैयार किया गया है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |

## उदाहरण

```csharp
using (var archive = new Lz4Archive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.lz4");
}
```

### संबंधित देखें

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

आर्काइव के भीतर संपीड़ित की जाने वाली सामग्री को सेट करता है।

```csharp
public void SetSource(FileInfo fileInfo)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| fileInfo | FileInfo | कम्प्रेस की जाने वाली फ़ाइल का संदर्भ। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| InvalidOperationException | आर्काइव को एक्सट्रैक्शन के लिए तैयार किया गया है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |

## उदाहरण

स्ट्रीम से एक आर्काइव खोलें और उसे `MemoryStream` में एक्सट्रैक्ट करें

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.lz4");
}
```

### संबंधित देखें

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(TarArchive, TarFormat) {#setsource}

आर्काइव के भीतर संपीड़ित की जाने वाली सामग्री को सेट करता है।

```csharp
public void SetSource(TarArchive tarArchive, TarFormat format = TarFormat.UsTar)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| tarArchive | TarArchive | संकुचित करने के लिए टार आर्काइव। |
| फ़ॉर्मेट | TarFormat | टार हेडर फ़ॉर्मेट को परिभाषित करता है। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| InvalidOperationException | यह आर्काइव एक्सट्रैक्शन के लिए तैयार किया गया है। |

## टिप्पणियाँ

संयुक्त tar.lz4 आर्काइव बनाने के लिए इस मेथड का उपयोग करें।

## उदाहरण

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var lz4Archive = new Lz4Archive())
    {
        lz4Archive.SetSource(tarArchive);
        lz4Archive.Save("archive.tar.lz4");
    }
}
```

### संबंधित देखें

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* enum [TarFormat](../../../aspose.zip.tar/tarformat/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

आर्काइव के भीतर संपीड़ित की जाने वाली सामग्री को सेट करता है।

```csharp
public void SetSource(string path)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| पथ | String | संकुचित करने वाली फ़ाइल का पथ। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *path* शून्य है। |
| SecurityException | कॉलर के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है |
| ArgumentException | *path* खाली है, केवल सफ़ेद स्थान शामिल हैं, या इसमें अमान्य अक्षर हैं। |
| UnauthorizedAccessException | *path* फ़ाइल तक पहुँच अस्वीकृत है। |
| PathTooLongException | निर्दिष्ट *path*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 अक्षरों से कम होने चाहिए, और फ़ाइल नाम 260 अक्षरों से कम होने चाहिए। |
| NotSupportedException | *path* पर फ़ाइल में स्ट्रिंग के मध्य में कोलन (:) है। |
| InvalidOperationException | यह आर्काइव एक्सट्रैक्शन के लिए तैयार किया गया है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |

## उदाहरण

फ़ाइल पथ से एक आर्काइव खोलें और उसे `MemoryStream` में निकालें

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### संबंधित देखें

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


