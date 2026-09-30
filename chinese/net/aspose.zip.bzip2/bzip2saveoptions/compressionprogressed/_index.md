---
title: "Bzip2SaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP for .NET API 参考"
description: "Bzip2SaveOptions 事件。当原始流的一部分被压缩时触发"
type: docs
weight: 40
url: /zh/net/aspose.zip.bzip2/bzip2saveoptions/compressionprogressed/
---
## Bzip2SaveOptions.CompressionProgressed event

在压缩原始流的一部分时引发。

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## 备注

在多线程模式下压缩时此事件不会被触发。

## 示例

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### 另请参阅

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)


