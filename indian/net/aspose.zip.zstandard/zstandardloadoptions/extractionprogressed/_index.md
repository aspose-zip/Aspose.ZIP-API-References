---
title: "ZstandardLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "ZstandardLoadOptions इवेंट। कुछ बाइट्स निकाले जाने पर बुलाए जाने वाले डेलीगेट को प्राप्त करता है या सेट करता है"
type: docs
weight: 30
url: /hi/net/aspose.zip.zstandard/zstandardloadoptions/extractionprogressed/
---
## ZstandardLoadOptions.ExtractionProgressed event

जब कुछ बाइट्स निकाले जा चुके हों तो बुलाए जाने वाले डेलीगेट को प्राप्त करता है या सेट करता है।

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## टिप्पणियाँ

इवेंट प्रेषक वह [`ZstandardArchive`](../../zstandardarchive/) इंस्टेंस है जिसका निष्कर्षण प्रगति पर है।

## उदाहरण

```csharp
ZstandardArchive archive = new ZstandardArchive("archive.zst", 
new ZStandardLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### संबंधित देखें

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardLoadOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardloadoptions/)
* assembly [Aspose.Zip](../../../)


