---
title: GzipArchive.SetSource
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: GzipArchive तरक. समग्र क संग्रह के भतर संपड़त करने के लए सेट करत है
type: docs
weight: 70
url: /hi/net/aspose.zip.gzip/gziparchive/setsource/
---
## SetSource(Stream) {#setsource_2}

सामग्री को संग्रह के भीतर संपीड़ित करने के लिए सेट करता है।

```csharp
public void SetSource(Stream source)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| source | Stream | संग्रह के लिए इनपुट स्ट्रीम। |

### उदाहरण

```csharp
using (var archive = new GzipArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.gz");
}
```

### यह सभी देखें

* class [GzipArchive](../)
* नाम स्थान [Aspose.Zip.Gzip](../../gziparchive/)
* सभा [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

सामग्री को संग्रह के भीतर संपीड़ित करने के लिए सेट करता है।

```csharp
public void SetSource(FileInfo fileInfo)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileInfo | FileInfo | संपीड़ित की जाने वाली फ़ाइल का संदर्भ। |

### उदाहरण

एक स्ट्रीम से एक संग्रह खोलें और इसे एक में निकालें`मेमोरीस्ट्रीम`

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.gz");
}
```

### यह सभी देखें

* class [GzipArchive](../)
* नाम स्थान [Aspose.Zip.Gzip](../../gziparchive/)
* सभा [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

सामग्री को संग्रह के भीतर संपीड़ित करने के लिए सेट करता है।

```csharp
public void SetSource(string path)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | String | फ़ाइल का पथ कंप्रेस किया जाना है. |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *path* शून्य है। |
| SecurityException | कॉल करने वाले के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *path* खाली है, केवल सफेद स्थान हैं, या अमान्य वर्ण हैं। |
| UnauthorizedAccessException | फ़ाइल तक पहुंच*path* वर्जित किया गया है। |
| PathTooLongException | विष्तृत*path*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 वर्णों से कम होने चाहिए और फ़ाइल नाम 260 वर्णों से कम होने चाहिए। |
| NotSupportedException | पर फाइल करें*path* स्ट्रिंग के बीच में एक कोलन (:) होता है। |

### उदाहरण

फ़ाइल से पथ द्वारा एक संग्रह खोलें और इसे एक में निकालें`मेमोरीस्ट्रीम`

```csharp
using (var archive = new GzipArchive()) 
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

## SetSource(TarArchive) {#setsource}

सामग्री को संग्रह के भीतर संपीड़ित करने के लिए सेट करता है।

```csharp
public void SetSource(TarArchive tarArchive)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| tarArchive | TarArchive | टार संग्रह को कंप्रेस किया जाना है। |

### टिप्पणियों

संयुक्त tar.gz संग्रह बनाने के लिए इस विधि का उपयोग करें।

### उदाहरण

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var gzippedArchive = new GzipArchive())
    {
           gzippedArchive.SetSource(tarArchive);
           gzippedArchive.Save("archive.tar.gz");
    }
}
```

### यह सभी देखें

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* class [GzipArchive](../)
* नाम स्थान [Aspose.Zip.Gzip](../../gziparchive/)
* सभा [Aspose.Zip](../../../)


