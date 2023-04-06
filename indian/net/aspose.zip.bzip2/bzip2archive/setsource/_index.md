---
title: Bzip2Archive.SetSource
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Bzip2Archive तरक. समग्र क संग्रह के भतर संपड़त करने के लए सेट करत है
type: docs
weight: 60
url: /hi/net/aspose.zip.bzip2/bzip2archive/setsource/
---
## SetSource(Stream) {#setsource_3}

सामग्री को संग्रह के भीतर संपीड़ित करने के लिए सेट करता है।

```csharp
public void SetSource(Stream source)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| source | Stream | संग्रह के लिए इनपुट स्ट्रीम। |

### उदाहरण

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00,0xFF }));
    archive.Save("archive.bz2");
}
```

### यह सभी देखें

* class [Bzip2Archive](../)
* नाम स्थान [Aspose.Zip.Bzip2](../../bzip2archive/)
* सभा [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_2}

सामग्री को संग्रह के भीतर संपीड़ित करने के लिए सेट करता है।

```csharp
public void SetSource(FileInfo fileInfo)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileInfo | FileInfo | संपीड़ित की जाने वाली फ़ाइल का संदर्भ। |

### उदाहरण

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.bz2");
}
```

### यह सभी देखें

* class [Bzip2Archive](../)
* नाम स्थान [Aspose.Zip.Bzip2](../../bzip2archive/)
* सभा [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_4}

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

## SetSource(TarArchive, TarFormat) {#setsource_1}

सामग्री को संग्रह के भीतर संपीड़ित करने के लिए सेट करता है।

```csharp
public void SetSource(TarArchive tarArchive, TarFormat format = TarFormat.UsTar)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| tarArchive | TarArchive | टार संग्रह को कंप्रेस किया जाना है। |
| format | TarFormat | टार हेडर प्रारूप को परिभाषित करता है। |

### टिप्पणियों

संयुक्त tar.bz2 संग्रह बनाने के लिए इस विधि का उपयोग करें।

### उदाहरण

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var bzippedArchive = new Bzip2Archive())
    {
        bzippedArchive.SetSource(tarArchive);
        bzippedArchive.Save("archive.tar.bz2");
    }
}
```

### यह सभी देखें

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* enum [TarFormat](../../../aspose.zip.tar/tarformat/)
* class [Bzip2Archive](../)
* नाम स्थान [Aspose.Zip.Bzip2](../../bzip2archive/)
* सभा [Aspose.Zip](../../../)

---

## SetSource(CpioArchive, CpioFormat) {#setsource}

सामग्री को संग्रह के भीतर संपीड़ित करने के लिए सेट करता है।

```csharp
public void SetSource(CpioArchive cpioArchive, CpioFormat format = CpioFormat.OldAscii)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| cpioArchive | CpioArchive | Cpio संग्रह को कंप्रेस किया जाना है. |
| format | CpioFormat | cpio हैडर प्रारूप को परिभाषित करता है। |

### टिप्पणियों

संयुक्त cpio.bz2 संग्रह बनाने के लिए इस विधि का उपयोग करें।

### उदाहरण

```csharp
using (var cpioArchive = new CpioArchive())
{
    cpioArchive.CreateEntry("first.bin", "data1.bin");
    cpioArchive.CreateEntry("second.bin", "data2.bin");
    using (var bzippedArchive = new Bzip2Archive())
    {
        bzippedArchive.SetSource(cpioArchive);
        bzippedArchive.Save("archive.cpio.bz2");
    }
}
```

### यह सभी देखें

* class [CpioArchive](../../../aspose.zip.cpio/cpioarchive/)
* enum [CpioFormat](../../../aspose.zip.cpio/cpioformat/)
* class [Bzip2Archive](../)
* नाम स्थान [Aspose.Zip.Bzip2](../../bzip2archive/)
* सभा [Aspose.Zip](../../../)


