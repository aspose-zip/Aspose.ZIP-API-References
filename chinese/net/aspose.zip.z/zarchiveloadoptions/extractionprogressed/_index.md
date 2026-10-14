---
title: "ZArchiveLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP for .NET API 参考"
description: "ZArchiveLoadOptions 事件。获取或设置在提取了一些字节时调用的委托"
type: docs
weight: 30
url: /zh/net/aspose.zip.z/zarchiveloadoptions/extractionprogressed/
---
## ZArchiveLoadOptions.ExtractionProgressed event

获取或设置在提取了一些字节时调用的委托。

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## 备注

事件发送者是 [`ZArchive`](../../zarchive/) 实例，其提取过程正在进行。

## 示例

```csharp
ZArchive archive = new ZArchive("archive.z", 
new ZArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### 另请参阅

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZArchiveLoadOptions](../)
* namespace [Aspose.Zip.Z](../../zarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


