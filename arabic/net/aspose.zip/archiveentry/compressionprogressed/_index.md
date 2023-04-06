---
title: ArchiveEntry.CompressionProgressed
second_title: Aspose.ZIP لمرجع .NET API
description: ArchiveEntry حدث. يتم رفعه عند ضغط جزء من التدفق الخام.
type: docs
weight: 80
url: /ar/net/aspose.zip/archiveentry/compressionprogressed/
---
## ArchiveEntry.CompressionProgressed event

يتم رفعه عند ضغط جزء من التدفق الخام.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### ملاحظات

مرسل الحدث هو ملف[`ArchiveEntry`](../) مثال.

### أمثلة

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### أنظر أيضا

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* مساحة الاسم [Aspose.Zip](../../archiveentry/)
* المجسم [Aspose.Zip](../../../)


