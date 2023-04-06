---
title: Archive.CreateEntry
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Archive तरक. संग्रह में एकल प्रवष्ट बनएं.
type: docs
weight: 50
url: /hi/net/aspose.zip/archive/createentry/
---
## CreateEntry(string, string, bool, ArchiveEntrySettings) {#createentry_3}

संग्रह में एकल प्रविष्टि बनाएं.

```csharp
public ArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| path | String | नई फ़ाइल का पूरी तरह से योग्य नाम, या संबंधित फ़ाइल नाम जिसे संपीड़ित किया जाना है। |
| openImmediately | Boolean | फ़ाइल को तुरंत खोलने पर सही, अन्यथा संग्रह सहेजने पर फ़ाइल खोलें. |
| newEntrySettings | ArchiveEntrySettings | जोड़े जाने के लिए उपयोग की जाने वाली संपीड़न और एन्क्रिप्शन सेटिंग्स[`ArchiveEntry`](../../archiveentry/) वस्तु। |

### प्रतिलाभ की मात्रा

ज़िप प्रविष्टि उदाहरण।

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

प्रवेश नाम पूरी तरह से भीतर सेट है*name* पैरामीटर। फ़ाइल नाम में प्रदान किया गया*path* पैरामीटर प्रविष्टि नाम को प्रभावित नहीं करता है।

अगर फ़ाइल तुरंत खोली जाती है*openImmediately* संग्रह सहेजे जाने तक यह पैरामीटर अवरुद्ध हो जाता है।

### उदाहरण

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### यह सभी देखें

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* नाम स्थान [Aspose.Zip](../../archive/)
* सभा [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings) {#createentry_1}

संग्रह में एकल प्रविष्टि बनाएं.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, 
    ArchiveEntrySettings newEntrySettings = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| source | Stream | प्रविष्टि के लिए इनपुट स्ट्रीम। |
| newEntrySettings | ArchiveEntrySettings | जोड़े जाने के लिए उपयोग की जाने वाली संपीड़न और एन्क्रिप्शन सेटिंग्स[`ArchiveEntry`](../../archiveentry/) वस्तु। |

### प्रतिलाभ की मात्रा

ज़िप प्रविष्टि उदाहरण।

### उदाहरण

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.zip");
}
```

### यह सभी देखें

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* नाम स्थान [Aspose.Zip](../../archive/)
* सभा [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool, ArchiveEntrySettings) {#createentry}

संग्रह में एकल प्रविष्टि बनाएं.

```csharp
public ArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| fileInfo | FileInfo | संपीड़ित की जाने वाली फ़ाइल का मेटाडेटा। |
| openImmediately | Boolean | फ़ाइल को तुरंत खोलने पर सही, अन्यथा संग्रह सहेजने पर फ़ाइल खोलें. |
| newEntrySettings | ArchiveEntrySettings | जोड़े जाने के लिए उपयोग की जाने वाली संपीड़न और एन्क्रिप्शन सेटिंग्स[`ArchiveEntry`](../../archiveentry/) वस्तु। |

### प्रतिलाभ की मात्रा

ज़िप प्रविष्टि उदाहरण।

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* केवल पढ़ने के लिए है या एक निर्देशिका है। |
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, जैसे कि मैप न की गई ड्राइव पर होना। |
| IOException | फाइल पहले से ही खुली हुई है। |

### टिप्पणियों

प्रवेश नाम पूरी तरह से भीतर सेट है*name* पैरामीटर। फ़ाइल नाम में प्रदान किया गया*fileInfo* पैरामीटर प्रविष्टि नाम को प्रभावित नहीं करता है।

अगर फ़ाइल तुरंत खोली जाती है*openImmediately* संग्रह सहेजे जाने तक यह पैरामीटर अवरुद्ध हो जाता है।

### उदाहरण

विभिन्न एन्क्रिप्शन विधियों और प्रत्येक पासवर्ड के साथ एन्क्रिप्ट की गई प्रविष्टियों के साथ संग्रह बनाएं।

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
        archive.CreateEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass2", EncryptionMethod.AES128)));
        archive.CreateEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass3", EncryptionMethod.AES256)));
        archive.Save(zipFile);
    }
}
```

### यह सभी देखें

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* नाम स्थान [Aspose.Zip](../../archive/)
* सभा [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings, FileSystemInfo) {#createentry_2}

संग्रह में एकल प्रविष्टि बनाएं.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, ArchiveEntrySettings newEntrySettings, 
    FileSystemInfo fileInfo)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| source | Stream | प्रविष्टि के लिए इनपुट स्ट्रीम। |
| newEntrySettings | ArchiveEntrySettings | जोड़े जाने के लिए उपयोग की जाने वाली संपीड़न और एन्क्रिप्शन सेटिंग्स[`ArchiveEntry`](../../archiveentry/) वस्तु। |
| fileInfo | FileSystemInfo | संपीड़ित की जाने वाली फ़ाइल या फ़ोल्डर का मेटाडेटा। |

### प्रतिलाभ की मात्रा

ज़िप प्रविष्टि उदाहरण।

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| InvalidOperationException | दोनों*source* और*fileInfo* शून्य हैं या*source*शून्य है और*fileInfo* निर्देशिका के लिए खड़ा है। |

### टिप्पणियों

प्रवेश नाम पूरी तरह से भीतर सेट है*name* पैरामीटर। फ़ाइल नाम में प्रदान किया गया*fileInfo* पैरामीटर प्रविष्टि नाम को प्रभावित नहीं करता है।

*fileInfo* उल्लेख कर सकते हैंDirectoryInfo यदि प्रविष्टि निर्देशिका है।

### उदाहरण

एन्क्रिप्टेड प्रविष्टि के साथ संग्रह लिखें।

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF} ), new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")), new FileInfo("data1.bin")); 
        archive.Save(zipFile);
    }
}
```

### यह सभी देखें

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* नाम स्थान [Aspose.Zip](../../archive/)
* सभा [Aspose.Zip](../../../)


