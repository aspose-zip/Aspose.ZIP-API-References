---
title: "IVolumeStreamProvider.VolumeCompleted"
second_title: "Aspose.ZIP for .NET API 参考"
description: "IVolumeStreamProvider 方法。在拆分多卷归档的某个卷写入完成后调用"
type: docs
weight: 20
url: /zh/net/aspose.zip.saving/ivolumestreamprovider/volumecompleted/
---
## IVolumeStreamProvider.VolumeCompleted method

在拆分（多卷）存档的卷写入后调用。

```csharp
public void VolumeCompleted(int index, Stream s, bool isLast)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| index | Int32 | 已写入的卷数量，从零开始计数。 |
| s | 流 | 卷写入的目标流。 |
| isLast | Boolean | 该卷是否结束归档。 |

### 另请参阅

* interface [IVolumeStreamProvider](../)
* namespace [Aspose.Zip.Saving](../../ivolumestreamprovider/)
* assembly [Aspose.Zip](../../../)


