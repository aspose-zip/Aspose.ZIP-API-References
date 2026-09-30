---
title: "LzmaArchiveSettings.CompressionProgressed"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "حدث LzmaArchiveSettings. يُثار عندما يتم ضغط جزء من تدفق البيانات الخام"
type: docs
weight: 50
url: /ar/net/aspose.zip.lzma/lzmaarchivesettings/compressionprogressed/
---
## LzmaArchiveSettings.CompressionProgressed event

يُرفع عندما يتم ضغط جزء من تدفق البيانات الخام.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## أمثلة

```csharp
lzmaArchiveSettings.CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### انظر أيضًا

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


