---
title: "ZstandardSaveOptions.CompressionProgressed"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "حدث ZstandardSaveOptions. يُثار عندما يتم ضغط جزء من تدفق البيانات الخام"
type: docs
weight: 20
url: /ar/net/aspose.zip.zstandard/zstandardsaveoptions/compressionprogressed/
---
## ZstandardSaveOptions.CompressionProgressed event

يُرفع عندما يتم ضغط جزء من تدفق البيانات الخام.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## أمثلة

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### انظر أيضًا

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardSaveOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardsaveoptions/)
* assembly [Aspose.Zip](../../../)


