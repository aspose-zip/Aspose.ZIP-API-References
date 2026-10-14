---
title: "XarLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP for .NET API 参考"
description: "XarLoadOptions 属性。获取或设置在提取了一些字节时调用的委托"
type: docs
weight: 30
url: /zh/net/aspose.zip.xar/xarloadoptions/entryextractionprogressed/
---
## XarLoadOptions.EntryExtractionProgressed property

获取或设置在提取了一些字节时调用的委托。

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## 备注

事件发送者是 [`XarFileEntry`](../../xarfileentry/) 实例，其提取已进展。

## 示例

```csharp
XarArchive archive = new XarArchive("archive.xar", 
new XarLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((XarFileEntry)s).Length); } })                 
```

### 另请参阅

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarLoadOptions](../)
* namespace [Aspose.Zip.Xar](../../xarloadoptions/)
* assembly [Aspose.Zip](../../../)


