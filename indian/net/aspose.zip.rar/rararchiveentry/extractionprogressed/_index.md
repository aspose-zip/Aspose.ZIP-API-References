---
title: RarArchiveEntry.ExtractionProgressed
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: RarArchiveEntry आयजन. अपरष्कृत धर के एक हस्से क नकले जने पर बढ़त है
type: docs
weight: 80
url: /hi/net/aspose.zip.rar/rararchiveentry/extractionprogressed/
---
## RarArchiveEntry.ExtractionProgressed event

अपरिष्कृत धारा के एक हिस्से को निकाले जाने पर बढ़ता है।

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### टिप्पणियों

घटना प्रेषक एक है[`RarArchiveEntry`](../) उदाहरण।

### उदाहरण

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((RarArchiveEntry)s).UncompressedSize); };
```

### यह सभी देखें

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [RarArchiveEntry](../)
* नाम स्थान [Aspose.Zip.Rar](../../rararchiveentry/)
* सभा [Aspose.Zip](../../../)


