---
title: SevenZipArchive.CreateEntry
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: SevenZipArchive तरक. संग्रह में एकल प्रवष्ट बनएं.
type: docs
weight: 50
url: /hi/net/aspose.zip.sevenzip/sevenziparchive/createentry/
---
## CreateEntry(string, FileInfo, bool, SevenZipEntrySettings) {#createentry}

संग्रह में एकल प्रविष्टि बनाएं.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, FileInfo fileInfo, 
    bool openImmediately = false, SevenZipEntrySettings newEntrySettings = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| fileInfo | FileInfo | संपीड़ित की जाने वाली फ़ाइल का मेटाडेटा। |
| openImmediately | Boolean | फ़ाइल को तुरंत खोलने पर सही, अन्यथा संग्रह सहेजने पर फ़ाइल खोलें. |
| newEntrySettings | SevenZipEntrySettings | जोड़े जाने के लिए उपयोग की जाने वाली संपीड़न और एन्क्रिप्शन सेटिंग्स[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) वस्तु। |

### प्रतिलाभ की मात्रा

सात ज़िप प्रविष्टि उदाहरण।

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

अलग-अलग पासवर्ड के साथ एन्क्रिप्ट की गई प्रविष्टियों के साथ संग्रह बनाएं।

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
        archive.CreateEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
        archive.CreateEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
        archive.Save(sevenZipFile);
    }
}
```

### यह सभी देखें

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* नाम स्थान [Aspose.Zip.SevenZip](../../sevenziparchive/)
* सभा [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings, FileSystemInfo) {#createentry_2}

संग्रह में एकल प्रविष्टि बनाएं.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings, FileSystemInfo fileInfo)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| source | Stream | प्रविष्टि के लिए इनपुट स्ट्रीम। |
| newEntrySettings | SevenZipEntrySettings | जोड़े जाने के लिए उपयोग की जाने वाली संपीड़न और एन्क्रिप्शन सेटिंग्स[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) वस्तु। |
| fileInfo | FileSystemInfo | संपीड़ित की जाने वाली फ़ाइल या फ़ोल्डर का मेटाडेटा। |

### प्रतिलाभ की मात्रा

SevenZip प्रविष्टि उदाहरण।

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| InvalidOperationException | दोनों*source* और*fileInfo* शून्य हैं या*source*शून्य है और*fileInfo* निर्देशिका के लिए खड़ा है। |

### टिप्पणियों

प्रवेश नाम पूरी तरह से भीतर सेट है*name* पैरामीटर। फ़ाइल नाम में प्रदान किया गया*fileInfo* पैरामीटर प्रविष्टि नाम को प्रभावित नहीं करता है।

*fileInfo* उल्लेख कर सकते हैंDirectoryInfo यदि प्रविष्टि निर्देशिका है।

### उदाहरण

LZMA2 संकुचित एन्क्रिप्टेड प्रविष्टि के साथ संग्रह लिखें।

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF}), new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1")), new FileInfo("data1.bin")); 
        archive.Save(sevenZipFile);
    }
}
```

### यह सभी देखें

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* नाम स्थान [Aspose.Zip.SevenZip](../../sevenziparchive/)
* सभा [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings) {#createentry_1}

संग्रह में एकल प्रविष्टि बनाएं.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| source | Stream | प्रविष्टि के लिए इनपुट स्ट्रीम। |
| newEntrySettings | SevenZipEntrySettings | जोड़े जाने के लिए उपयोग की जाने वाली संपीड़न और एन्क्रिप्शन सेटिंग्स[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) वस्तु। |

### प्रतिलाभ की मात्रा

ज़िप प्रविष्टि उदाहरण।

### उदाहरण

LZMA2 संपीड़न और सभी प्रविष्टियों के एन्क्रिप्शन के साथ 7z संग्रह लिखें।

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.7z");
}
```

### यह सभी देखें

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* नाम स्थान [Aspose.Zip.SevenZip](../../sevenziparchive/)
* सभा [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, SevenZipEntrySettings) {#createentry_3}

संग्रह में एकल प्रविष्टि बनाएं.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    SevenZipEntrySettings newEntrySettings = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| path | String | नई फ़ाइल का पूरी तरह से योग्य नाम, या संबंधित फ़ाइल नाम जिसे संपीड़ित किया जाना है। |
| openImmediately | Boolean | फ़ाइल को तुरंत खोलने पर सही, अन्यथा संग्रह सहेजने पर फ़ाइल खोलें. |
| newEntrySettings | SevenZipEntrySettings | जोड़े जाने के लिए उपयोग की जाने वाली संपीड़न और एन्क्रिप्शन सेटिंग्स[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) वस्तु। |

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
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings())))
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### यह सभी देखें

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* नाम स्थान [Aspose.Zip.SevenZip](../../sevenziparchive/)
* सभा [Aspose.Zip](../../../)


