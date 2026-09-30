---
title: "Bzip2SaveOptions.CompressionProgressed"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "حدث Bzip2SaveOptions. يُطلق عندما يتم ضغط جزء من الدفق الخام"
type: docs
weight: 40
url: /ar/net/aspose.zip.bzip2/bzip2saveoptions/compressionprogressed/
---
## Bzip2SaveOptions.CompressionProgressed event

يُرفع عندما يتم ضغط جزء من تدفق البيانات الخام.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## ملاحظات

هذا الحدث لن يُطلق عند الضغط في وضع متعدد الخيوط.

## أمثلة

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### انظر أيضًا

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)


