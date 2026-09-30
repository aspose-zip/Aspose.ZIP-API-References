---
title: "ZArchiveLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "ZArchiveLoadOptions इवेंट। जब कुछ बाइट्स निकाले गए हों तो बुलाए जाने वाले डेलीगेट को प्राप्त या सेट करता है"
type: docs
weight: 30
url: /hi/net/aspose.zip.z/zarchiveloadoptions/extractionprogressed/
---
## ZArchiveLoadOptions.ExtractionProgressed event

जब कुछ बाइट्स निकाले जा चुके हों तो बुलाए जाने वाले डेलीगेट को प्राप्त करता है या सेट करता है।

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## टिप्पणियाँ

इवेंट प्रेषक वह [`ZArchive`](../../zarchive/) इंस्टेंस है जिसका निष्कर्षण प्रगति पर है।

## उदाहरण

```csharp
ZArchive archive = new ZArchive("archive.z", 
new ZArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### संबंधित देखें

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZArchiveLoadOptions](../)
* namespace [Aspose.Zip.Z](../../zarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


