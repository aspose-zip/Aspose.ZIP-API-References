---
title: ArchiveEntry.ExtractionProgressed
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: ArchiveEntry आयजन. अपरष्कृत धर के एक हस्से क नकले जने पर बढ़त है
type: docs
weight: 90
url: /hi/net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

अपरिष्कृत धारा के एक हिस्से को निकाले जाने पर बढ़ता है।

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### टिप्पणियों

घटना प्रेषक एक है[`ArchiveEntry`](../) उदाहरण।

### उदाहरण

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

### यह सभी देखें

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* नाम स्थान [Aspose.Zip](../../archiveentry/)
* सभा [Aspose.Zip](../../../)


