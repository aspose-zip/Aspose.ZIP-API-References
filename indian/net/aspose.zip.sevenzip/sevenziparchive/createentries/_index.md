---
title: SevenZipArchive.CreateEntries
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: SevenZipArchive तरक. दए गए नर्देशक में सभ फइलं और नर्देशकओं क पुनरवर्त रूप से संग्रह में जड़त है
type: docs
weight: 40
url: /hi/net/aspose.zip.sevenzip/sevenziparchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

दिए गए निर्देशिका में सभी फाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है।

```csharp
public SevenZipArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| directory | DirectoryInfo | संपीड़ित करने के लिए निर्देशिका। |
| includeRootDirectory | Boolean | इंगित करता है कि रूट निर्देशिका को स्वयं शामिल करना है या नहीं। |

### प्रतिलाभ की मात्रा

रचित प्रविष्टियों के साथ संग्रह।

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| DirectoryNotFoundException | करने का मार्ग*directory* अमान्य है, जैसे कि मैप न की गई ड्राइव पर होना। |
| SecurityException | कॉल करने वाले के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है*directory*. |

### उदाहरण

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.7z");
}
```

### यह सभी देखें

* class [SevenZipArchive](../)
* नाम स्थान [Aspose.Zip.SevenZip](../../sevenziparchive/)
* सभा [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

दिए गए निर्देशिका में सभी फाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है।

```csharp
public SevenZipArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceDirectory | String | संपीड़ित करने के लिए निर्देशिका। |
| includeRootDirectory | Boolean | इंगित करता है कि रूट निर्देशिका को स्वयं शामिल करना है या नहीं। |

### प्रतिलाभ की मात्रा

रचित प्रविष्टियों के साथ संग्रह।

### उदाहरण

LZMA2 संपीड़न के साथ 7z संग्रह लिखें।

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.7z");
}
```

### यह सभी देखें

* class [SevenZipArchive](../)
* नाम स्थान [Aspose.Zip.SevenZip](../../sevenziparchive/)
* सभा [Aspose.Zip](../../../)


