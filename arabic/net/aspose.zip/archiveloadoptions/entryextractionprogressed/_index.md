---
title: ArchiveLoadOptions.EntryExtractionProgressed
second_title: Aspose.ZIP لمرجع .NET API
description: ArchiveLoadOptions ملكية. الحصول على المفوض الذي تم استدعاؤه أو تعيينه عند استخراج بعض البايت.
type: docs
weight: 40
url: /ar/net/aspose.zip/archiveloadoptions/entryextractionprogressed/
---
## ArchiveLoadOptions.EntryExtractionProgressed property

الحصول على المفوض الذي تم استدعاؤه أو تعيينه عند استخراج بعض البايت.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

### ملاحظات

مرسل الحدث هو[`ArchiveEntry`](../../archiveentry/) المثال الذي تقدم فيه الاستخراج.

### أمثلة

```csharp
Archive archive = new Archive("archive.zip", 
new ArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); } })                 
```

### أنظر أيضا

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveLoadOptions](../)
* مساحة الاسم [Aspose.Zip](../../archiveloadoptions/)
* المجسم [Aspose.Zip](../../../)


