---
title: "Bzip2LoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP for .NET API 参考"
description: "Bzip2LoadOptions 事件。事件在提取了一些字节时被触发"
type: docs
weight: 30
url: /zh/net/aspose.zip.bzip2/bzip2loadoptions/extractionprogressed/
---
## Bzip2LoadOptions.ExtractionProgressed event

在提取了一些字节时触发的事件。

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## 备注

事件发送者是 [`Bzip2Archive`](../../bzip2archive/) 实例，其提取正在进行。[`ProceededBytes`](../../../aspose.zip/progresseventargs/proceededbytes/) 是提取后的字节数。

## 示例

```csharp
Bzip2LoadOptions loadOptions = new Bzip2LoadOptions(); 
loadOptions.ExtractionProgressed += (s, e) => { percent = (int) ((double)(100 * e.ProceededBytes) / originalFileLength); };
```

### 另请参阅

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2LoadOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2loadoptions/)
* assembly [Aspose.Zip](../../../)


