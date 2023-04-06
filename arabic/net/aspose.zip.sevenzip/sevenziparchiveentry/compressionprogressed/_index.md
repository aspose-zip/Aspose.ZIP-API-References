---
title: SevenZipArchiveEntry.CompressionProgressed
second_title: Aspose.ZIP لمرجع .NET API
description: SevenZipArchiveEntry حدث. يتم رفعه عند ضغط جزء من التدفق الخام.
type: docs
weight: 70
url: /ar/net/aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/
---
## SevenZipArchiveEntry.CompressionProgressed event

يتم رفعه عند ضغط جزء من التدفق الخام.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### ملاحظات

مرسل الحدث هو ملف[`SevenZipArchiveEntry`](../) مثال.

### أمثلة

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### أنظر أيضا

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [SevenZipArchiveEntry](../)
* مساحة الاسم [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* المجسم [Aspose.Zip](../../../)


