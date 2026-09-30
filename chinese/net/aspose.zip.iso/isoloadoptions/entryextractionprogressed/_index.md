---
title: "IsoLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP for .NET API 参考"
description: "IsoLoadOptions 属性。获取或设置在提取一定字节后被调用的委托"
type: docs
weight: 30
url: /zh/net/aspose.zip.iso/isoloadoptions/entryextractionprogressed/
---
## IsoLoadOptions.EntryExtractionProgressed property

获取或设置在提取了一些字节时调用的委托。

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## 备注

事件发送者是 [`IsoEntry`](../../isoentry/) 实例，其提取过程已进展。

## 示例

```csharp
IsoArchive archive = new IsoArchive("archive.iso", 
new IsoLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })                 
```

### 另请参阅

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [IsoLoadOptions](../)
* namespace [Aspose.Zip.Iso](../../isoloadoptions/)
* assembly [Aspose.Zip](../../../)


