---
title: "ZArchiveSaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP for .NET API 参考"
description: "ZArchiveSaveOptions 事件。当压缩一部分原始流时触发"
type: docs
weight: 20
url: /zh/net/aspose.zip.z/zarchivesaveoptions/compressionprogressed/
---
## ZArchiveSaveOptions.CompressionProgressed event

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
* class [ZArchiveSaveOptions](../)
* namespace [Aspose.Zip.Z](../../zarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


