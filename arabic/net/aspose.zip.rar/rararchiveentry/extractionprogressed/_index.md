---
title: RarArchiveEntry.ExtractionProgressed
second_title: Aspose.ZIP لمرجع .NET API
description: RarArchiveEntry حدث. يتم رفعه عند استخراج جزء من الدفق الخام.
type: docs
weight: 80
url: /ar/net/aspose.zip.rar/rararchiveentry/extractionprogressed/
---
## RarArchiveEntry.ExtractionProgressed event

يتم رفعه عند استخراج جزء من الدفق الخام.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### ملاحظات

مرسل الحدث هو ملف[`RarArchiveEntry`](../) مثال.

### أمثلة

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((RarArchiveEntry)s).UncompressedSize); };
```

### أنظر أيضا

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [RarArchiveEntry](../)
* مساحة الاسم [Aspose.Zip.Rar](../../rararchiveentry/)
* المجسم [Aspose.Zip](../../../)


