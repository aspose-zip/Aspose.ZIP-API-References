---
title: "IsoLoadOptions.EntryExtractionProgressed"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "خاصية IsoLoadOptions. تحصل أو تعين المفوض الذي يُستدعى عندما يتم استخراج بعض البايتات"
type: docs
weight: 30
url: /ar/net/aspose.zip.iso/isoloadoptions/entryextractionprogressed/
---
## IsoLoadOptions.EntryExtractionProgressed property

يحصل أو يعيّن المفوض الذي يُستدعى عندما يتم استخراج بعض البايتات.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## ملاحظات

مرسل الحدث هو كائن [`IsoEntry`](../../isoentry/) الذي يتم فيه تقدم الاستخراج.

## أمثلة

```csharp
IsoArchive archive = new IsoArchive("archive.iso", 
new IsoLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })                 
```

### انظر أيضًا

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [IsoLoadOptions](../)
* namespace [Aspose.Zip.Iso](../../isoloadoptions/)
* assembly [Aspose.Zip](../../../)


