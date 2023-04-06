---
title: SevenZipArchiveEntry.CompressionProgressed
second_title: Aspose.ZIP for .NET API 参考
description: SevenZipArchiveEntry 事件. 在压缩原始流的一部分时引发
type: docs
weight: 70
url: /zh/net/aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/
---
## SevenZipArchiveEntry.CompressionProgressed event

在压缩原始流的一部分时引发。

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### 评论

事件发送者是[`SevenZipArchiveEntry`](../)实例。

### 例子

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### 也可以看看

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [SevenZipArchiveEntry](../)
* 命名空间 [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* 部件 [Aspose.Zip](../../../)


