---
title: ArchiveLoadOptions.EntryExtractionProgressed
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: ArchiveLoadOptions संपत्त. कुछ बइट नकले जने पर प्रतनध क बुलय जत है य सेट करत है
type: docs
weight: 40
url: /hi/net/aspose.zip/archiveloadoptions/entryextractionprogressed/
---
## ArchiveLoadOptions.EntryExtractionProgressed property

कुछ बाइट निकाले जाने पर प्रतिनिधि को बुलाया जाता है या सेट करता है।

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

### टिप्पणियों

घटना प्रेषक है[`ArchiveEntry`](../../archiveentry/) उदाहरण जो निष्कर्षण प्रगति की है।

### उदाहरण

```csharp
Archive archive = new Archive("archive.zip", 
new ArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); } })                 
```

### यह सभी देखें

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveLoadOptions](../)
* नाम स्थान [Aspose.Zip](../../archiveloadoptions/)
* सभा [Aspose.Zip](../../../)


