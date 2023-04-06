---
title: TarArchive.DeleteEntry
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: TarArchive तरक. प्रवष्टयं क सूच से कस वशष्ट प्रवष्ट क पहल घटन क हटत है
type: docs
weight: 90
url: /hi/net/aspose.zip.tar/tararchive/deleteentry/
---
## DeleteEntry(TarEntry) {#deleteentry}

प्रविष्टियों की सूची से किसी विशिष्ट प्रविष्टि की पहली घटना को हटाता है।

```csharp
public TarArchive DeleteEntry(TarEntry entry)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| entry | TarEntry | प्रविष्टियों की सूची से निकालने के लिए प्रविष्टि। |

### प्रतिलाभ की मात्रा

प्रविष्टि वाला संग्रह हटाया गया.

### उदाहरण

यहां बताया गया है कि आप अंतिम प्रविष्टि को छोड़कर सभी प्रविष्टियां कैसे निकाल सकते हैं:

```csharp
using (var archive = new TarArchive("archive.tar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputTarFile);
}
```

### यह सभी देखें

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* नाम स्थान [Aspose.Zip.Tar](../../tararchive/)
* सभा [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

इंडेक्स द्वारा प्रविष्टियों की सूची से प्रविष्टि को हटाता है।

```csharp
public TarArchive DeleteEntry(int entryIndex)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| entryIndex | Int32 | निकालने के लिए प्रविष्टि का शून्य-आधारित अनुक्रमणिका। |

### प्रतिलाभ की मात्रा

प्रविष्टि वाला संग्रह हटाया गया.

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex* 0.-या- से कम है*entryIndex* के बराबर या उससे अधिक है`प्रविष्टियां` गिनती करना। |

### उदाहरण

```csharp
using (var archive = new TarArchive("two_files.tar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.tar");
}
```

### यह सभी देखें

* class [TarArchive](../)
* नाम स्थान [Aspose.Zip.Tar](../../tararchive/)
* सभा [Aspose.Zip](../../../)


