---
title: "ZstandardLoadOptions.ExtractionProgressed"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "حدث ZstandardLoadOptions. يحصل أو يعين المفوض الذي يُستدعى عندما يتم استخراج بعض البايتات"
type: docs
weight: 30
url: /ar/net/aspose.zip.zstandard/zstandardloadoptions/extractionprogressed/
---
## ZstandardLoadOptions.ExtractionProgressed event

يحصل أو يعيّن المفوض الذي يُستدعى عندما يتم استخراج بعض البايتات.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## ملاحظات

مرسل الحدث هو الكائن [`ZstandardArchive`](../../zstandardarchive/) الذي يتم فيه تقدم الاستخراج.

## أمثلة

```csharp
ZstandardArchive archive = new ZstandardArchive("archive.zst", 
new ZStandardLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### انظر أيضًا

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardLoadOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardloadoptions/)
* assembly [Aspose.Zip](../../../)


