---
title: XzArchiveSettings.XzArchiveSettings
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: XzArchiveSettings नर्मत. क एक नय उदहरण प्ररंभ करत हैXzArchiveSettings वर्ग एकल LZMA2 संपड़न क उपयग कर रह है
type: docs
weight: 10
url: /hi/net/aspose.zip.xz.settings/xzarchivesettings/xzarchivesettings/
---
## XzArchiveSettings() {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`XzArchiveSettings`](../) वर्ग एकल LZMA2 संपीड़न का उपयोग कर रहा है।

```csharp
public XzArchiveSettings()
```

### टिप्पणियों

LZMA2 फ़िल्टर आकार में डिफ़ॉल्ट शब्दकोश 16 मेगाबाइट के बराबर है, डिफ़ॉल्ट ब्लॉक आकार 64 मेगाबाइट के बराबर है, डिफ़ॉल्ट चेकसम प्रकार CRC32. है

### यह सभी देखें

* class [XzArchiveSettings](../)
* नाम स्थान [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* सभा [Aspose.Zip](../../../)

---

## XzArchiveSettings(XzFilterSettings[], long, XzCheckType) {#constructor_1}

का एक नया उदाहरण प्रारंभ करता है[`XzArchiveSettings`](../) वर्ग कस्टम पैरामीटर के साथ.

```csharp
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filters | XzFilterSettings[] | फ़िल्टर (कंप्रेसर) बनाने के लिए क्रमिक रूप से लागू किया जाना है[`XzArchive`](../../../aspose.zip.xz/xzarchive/) . यह या तो सिंगल हो सकता है[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) या की जोड़ी[`XzBcjX86FilterSettings`](../../xzbcjx86filtersettings/) और[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) |
| blockSize | Int64 | आकार xz संग्रह ब्लॉक। |
| checkType | XzCheckType | असम्पीडित डेटा के लिए चेकसम गणना का प्रकार। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentOutOfRangeException | *blockSize* नकारात्मक है। |
| ArgumentNullException | *filters* शून्य है |
| ArgumentException | *filters* एक से कम या दो से अधिक फ़िल्टर हैं, या अंतिम फ़िल्टर नहीं है[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/). |

### उदाहरण

```csharp
using (FileStream xzFile = File.Open("archive.xz", FileMode.Create))
{
    XzLZMA2FilterSettings filter = new XzLZMA2FilterSettings(5242880);
    XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {filter}, 10485760, XzCheckType.Crc32);
    using (var archive = new XzArchive(settings))
    {
        archive.SetSource("data.bin");
        archive.Save(xzFile);
     }
}
```

### यह सभी देखें

* class [XzFilterSettings](../../xzfiltersettings/)
* enum [XzCheckType](../../xzchecktype/)
* class [XzArchiveSettings](../)
* नाम स्थान [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* सभा [Aspose.Zip](../../../)


