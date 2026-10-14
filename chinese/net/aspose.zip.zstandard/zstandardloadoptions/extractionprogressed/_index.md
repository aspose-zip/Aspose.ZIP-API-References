---
title: "ZstandardLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP for .NET API 参考"
description: "ZstandardLoadOptions 事件。获取或设置在提取一定字节后被调用的委托"
type: docs
weight: 30
url: /zh/net/aspose.zip.zstandard/zstandardloadoptions/extractionprogressed/
---
## ZstandardLoadOptions.ExtractionProgressed event

获取或设置在提取了一些字节时调用的委托。

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## 备注

事件发送者是 [`ZstandardArchive`](../../zstandardarchive/) 实例，其提取正在进行。

## 示例

```csharp
ZstandardArchive archive = new ZstandardArchive("archive.zst", 
new ZStandardLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### 另请参阅

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardLoadOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardloadoptions/)
* assembly [Aspose.Zip](../../../)


