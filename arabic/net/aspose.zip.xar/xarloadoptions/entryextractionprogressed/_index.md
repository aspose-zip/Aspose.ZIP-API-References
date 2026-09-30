---
title: "XarLoadOptions.EntryExtractionProgressed"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "خاصية XarLoadOptions. تحصل أو تعيين المفوض الذي يُستدعى عندما يتم استخراج بعض البايتات"
type: docs
weight: 30
url: /ar/net/aspose.zip.xar/xarloadoptions/entryextractionprogressed/
---
## XarLoadOptions.EntryExtractionProgressed property

يحصل أو يعيّن المفوض الذي يُستدعى عندما يتم استخراج بعض البايتات.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## ملاحظات

مرسل الحدث هو كائن [`XarFileEntry`](../../xarfileentry/) الذي يتم تقدم استخراجها.

## أمثلة

```csharp
XarArchive archive = new XarArchive("archive.xar", 
new XarLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((XarFileEntry)s).Length); } })                 
```

### انظر أيضًا

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarLoadOptions](../)
* namespace [Aspose.Zip.Xar](../../xarloadoptions/)
* assembly [Aspose.Zip](../../../)


