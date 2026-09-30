---
title: "XarLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "XarLoadOptions प्रॉपर्टी। जब कुछ बाइट्स निकाले गए हों तो बुलाए जाने वाले डेलीगेट को प्राप्त या सेट करता है"
type: docs
weight: 30
url: /hi/net/aspose.zip.xar/xarloadoptions/entryextractionprogressed/
---
## XarLoadOptions.EntryExtractionProgressed property

जब कुछ बाइट्स निकाले जा चुके हों तो बुलाए जाने वाले डेलीगेट को प्राप्त करता है या सेट करता है।

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## टिप्पणियाँ

इवेंट प्रेषक वह [`XarFileEntry`](../../xarfileentry/) इंस्टेंस है जिसका निष्कर्षण प्रगति पर है।

## उदाहरण

```csharp
XarArchive archive = new XarArchive("archive.xar", 
new XarLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((XarFileEntry)s).Length); } })                 
```

### संबंधित देखें

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarLoadOptions](../)
* namespace [Aspose.Zip.Xar](../../xarloadoptions/)
* assembly [Aspose.Zip](../../../)


