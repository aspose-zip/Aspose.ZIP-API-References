---
title: "ZArchiveLoadOptions.ExtractionProgressed"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "حدث ZArchiveLoadOptions. يحصل أو يضبط المندوب الذي يُستدعى عندما يتم استخراج بعض البايتات"
type: docs
weight: 30
url: /ar/net/aspose.zip.z/zarchiveloadoptions/extractionprogressed/
---
## ZArchiveLoadOptions.ExtractionProgressed event

يحصل أو يعيّن المفوض الذي يُستدعى عندما يتم استخراج بعض البايتات.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## ملاحظات

مرسل الحدث هو كائن [`ZArchive`](../../zarchive/) الذي يتم فيه تقدم الاستخراج.

## أمثلة

```csharp
ZArchive archive = new ZArchive("archive.z", 
new ZArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### انظر أيضًا

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZArchiveLoadOptions](../)
* namespace [Aspose.Zip.Z](../../zarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


