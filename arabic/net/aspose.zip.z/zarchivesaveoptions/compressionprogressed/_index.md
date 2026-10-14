---
title: "ZArchiveSaveOptions.CompressionProgressed"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "حدث ZArchiveSaveOptions. يُثار عندما يتم ضغط جزء من تدفق البيانات الخام"
type: docs
weight: 20
url: /ar/net/aspose.zip.z/zarchivesaveoptions/compressionprogressed/
---
## ZArchiveSaveOptions.CompressionProgressed event

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
* class [ZArchiveSaveOptions](../)
* namespace [Aspose.Zip.Z](../../zarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


