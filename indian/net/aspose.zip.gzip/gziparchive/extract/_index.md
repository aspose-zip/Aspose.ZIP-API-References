---
title: GzipArchive.Extract
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: GzipArchive तरक. संग्रह क प्रदन क गई स्ट्रम में नकलत है
type: docs
weight: 40
url: /hi/net/aspose.zip.gzip/gziparchive/extract/
---
## GzipArchive.Extract method

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
using (var archive = new GzipArchive("archive.gz"))
{
     archive.Extract(httpResponseStream);
}
```

### यह सभी देखें

* class [GzipArchive](../)
* नाम स्थान [Aspose.Zip.Gzip](../../gziparchive/)
* सभा [Aspose.Zip](../../../)


