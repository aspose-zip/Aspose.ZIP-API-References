---
title: Bzip2Archive.Extract
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Bzip2Archive तरक. संग्रह क प्रदन क गई स्ट्रम में नकलत है
type: docs
weight: 30
url: /hi/net/aspose.zip.bzip2/bzip2archive/extract/
---
## Bzip2Archive.Extract method

संग्रह को प्रदान की गई स्ट्रीम में निकालता है।

```csharp
public void Extract(Stream destination)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destination | Stream | गंतव्य धारा। लिखने योग्य होना चाहिए। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentException | *destination* लिखने का समर्थन नहीं करता। |

### उदाहरण

```csharp
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
{
     archive.Extract(httpResponseStream);
}
```

### यह सभी देखें

* class [Bzip2Archive](../)
* नाम स्थान [Aspose.Zip.Bzip2](../../bzip2archive/)
* सभा [Aspose.Zip](../../../)


