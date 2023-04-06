---
title: ArchiveEntry.ExtractionProgressed
second_title: Aspose.ZIP لمرجع .NET API
description: ArchiveEntry حدث. يتم رفعه عند استخراج جزء من الدفق الخام.
type: docs
weight: 90
url: /ar/net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

يتم رفعه عند استخراج جزء من الدفق الخام.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### ملاحظات

مرسل الحدث هو ملف[`ArchiveEntry`](../) مثال.

### أمثلة

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

### أنظر أيضا

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* مساحة الاسم [Aspose.Zip](../../archiveentry/)
* المجسم [Aspose.Zip](../../../)


