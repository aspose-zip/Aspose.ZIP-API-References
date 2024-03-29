---
title: CpioArchive.DeleteEntry
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: CpioArchive तरक. प्रवष्टयं क सूच से कस वशष्ट प्रवष्ट क पहल घटन क हटत है
type: docs
weight: 50
url: /hi/net/aspose.zip.cpio/cpioarchive/deleteentry/
---
## DeleteEntry(CpioEntry) {#deleteentry}

प्रविष्टियों की सूची से किसी विशिष्ट प्रविष्टि की पहली घटना को हटाता है।

```csharp
public CpioArchive DeleteEntry(CpioEntry entry)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| entry | CpioEntry | प्रविष्टियों की सूची से निकालने के लिए प्रविष्टि। |

### प्रतिलाभ की मात्रा

Cpio प्रविष्टि उदाहरण।

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *entry* शून्य है। |

### उदाहरण

यहां बताया गया है कि आप अंतिम प्रविष्टि को छोड़कर सभी प्रविष्टियां कैसे निकाल सकते हैं:

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputCpioFile);
}
```

### यह सभी देखें

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* नाम स्थान [Aspose.Zip.Cpio](../../cpioarchive/)
* सभा [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

इंडेक्स द्वारा प्रविष्टियों की सूची से प्रविष्टि को हटाता है।

```csharp
public CpioArchive DeleteEntry(int entryIndex)
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
using (var archive = new CpioArchive("two_files.cpio"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.cpio");
}
```

### यह सभी देखें

* class [CpioArchive](../)
* नाम स्थान [Aspose.Zip.Cpio](../../cpioarchive/)
* सभा [Aspose.Zip](../../../)


