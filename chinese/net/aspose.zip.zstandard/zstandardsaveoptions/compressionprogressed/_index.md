---
title: "ZstandardSaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP for .NET API 参考"
description: "ZstandardSaveOptions 事件。当原始流的一部分被压缩时触发"
type: docs
weight: 20
url: /zh/net/aspose.zip.zstandard/zstandardsaveoptions/compressionprogressed/
---
## ZstandardSaveOptions.CompressionProgressed event

在压缩原始流的一部分时引发。

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## 示例

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### 另请参阅

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardSaveOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardsaveoptions/)
* assembly [Aspose.Zip](../../../)


