---
title: SevenZipArchiveEntry.CompressionProgressed
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: SevenZipArchiveEntry आयजन. अपरष्कृत धर के एक हस्से के संकुचत हने पर उठत है
type: docs
weight: 70
url: /hi/net/aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/
---
## SevenZipArchiveEntry.CompressionProgressed event

अपरिष्कृत धारा के एक हिस्से के संकुचित होने पर उठता है।

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### टिप्पणियों

घटना प्रेषक एक है[`SevenZipArchiveEntry`](../) उदाहरण।

### उदाहरण

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### यह सभी देखें

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [SevenZipArchiveEntry](../)
* नाम स्थान [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* सभा [Aspose.Zip](../../../)


