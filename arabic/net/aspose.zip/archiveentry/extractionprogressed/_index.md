---
title: ExtractionProgressed
second_title: Aspose.ZIP لمرجع .NET API
description: يتم رفعه عند استخراج جزء من الدفق الخام.
type: docs
weight: 80
url: /ar/net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

يتم رفعه عند استخراج جزء من الدفق الخام.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### ملاحظات

مرسل الحدث هو ملف[`ArchiveEntry`](../../archiveentry) نموذج.

### أمثلة

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

### أنظر أيضا

* class [ProgressEventArgs](../../progresseventargs)
* class [ArchiveEntry](../../archiveentry)
* مساحة الاسم [Aspose.Zip](../../archiveentry)
* المجسم [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->