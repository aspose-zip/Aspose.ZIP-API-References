---
title: Archive.DeleteEntry
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Archive तरक. प्रवष्टयं क सूच से कस वशष्ट प्रवष्ट क पहल घटन क हटत है
type: docs
weight: 60
url: /hi/net/aspose.zip/archive/deleteentry/
---
## DeleteEntry(ArchiveEntry) {#deleteentry}

प्रविष्टियों की सूची से किसी विशिष्ट प्रविष्टि की पहली घटना को हटाता है।

```csharp
public Archive DeleteEntry(ArchiveEntry entry)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| entry | ArchiveEntry | प्रविष्टियों की सूची से निकालने के लिए प्रविष्टि। |

### प्रतिलाभ की मात्रा

प्रविष्टि वाला संग्रह हटाया गया.

### उदाहरण

यहां बताया गया है कि आप अंतिम प्रविष्टि को छोड़कर सभी प्रविष्टियां कैसे निकाल सकते हैं:

```csharp
using (var archive = new Archive("archive.zip"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save("last_entry.zip");
}
```

### यह सभी देखें

* class [ArchiveEntry](../../archiveentry/)
* class [Archive](../)
* नाम स्थान [Aspose.Zip](../../archive/)
* सभा [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

इंडेक्स द्वारा प्रविष्टियों की सूची से प्रविष्टि को हटाता है।

```csharp
public Archive DeleteEntry(int entryIndex)
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
using (var archive = new TarArchive("two_files.zip"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.zip");
}
```

### यह सभी देखें

* class [Archive](../)
* नाम स्थान [Aspose.Zip](../../archive/)
* सभा [Aspose.Zip](../../../)


