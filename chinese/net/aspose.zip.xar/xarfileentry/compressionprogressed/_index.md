---
title: "XarFileEntry.CompressionProgressed"
second_title: "Aspose.ZIP for .NET API 参考"
description: "XarFileEntry 事件。当原始流的一部分被压缩时触发"
type: docs
weight: 20
url: /zh/net/aspose.zip.xar/xarfileentry/compressionprogressed/
---
## XarFileEntry.CompressionProgressed event

在压缩原始流的一部分时引发。

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## 备注

事件发送者是一个 [`XarFileEntry`](../) 实例。

## 示例

```csharp
archive.Entries.First().CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### 另请参阅

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
* assembly [Aspose.Zip](../../../)


