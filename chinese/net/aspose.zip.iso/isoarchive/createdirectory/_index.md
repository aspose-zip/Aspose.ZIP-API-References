---
title: "IsoArchive.CreateDirectory"
second_title: "Aspose.ZIP for .NET API 参考"
description: "IsoArchive 方法。向 ISO 镜像添加目录"
type: docs
weight: 30
url: /zh/net/aspose.zip.iso/isoarchive/createdirectory/
---
## IsoArchive.CreateDirectory method

向 ISO 镜像添加目录。

```csharp
public IsoEntry CreateDirectory(string name)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | String | ISO 中目录的路径。 |

### Return Value

已组成 ISO 条目。

### 异常

| 异常 | 条件 |
| --- | --- |
| InvalidOperationException | 存档已打开用于提取。 |
| ArgumentNullException | `name` 为 null 或为空。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |

### 另请参阅

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


