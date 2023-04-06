---
title: ArchiveEntry.CompressionProgressed
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: ArchiveEntry आयजन. अपरष्कृत धर के एक हस्से के संकुचत हने पर उठत है
type: docs
weight: 80
url: /hi/net/aspose.zip/archiveentry/compressionprogressed/
---
## ArchiveEntry.CompressionProgressed event

अपरिष्कृत धारा के एक हिस्से के संकुचित होने पर उठता है।

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### टिप्पणियों

घटना प्रेषक एक है[`ArchiveEntry`](../) उदाहरण।

### उदाहरण

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### यह सभी देखें

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* नाम स्थान [Aspose.Zip](../../archiveentry/)
* सभा [Aspose.Zip](../../../)


