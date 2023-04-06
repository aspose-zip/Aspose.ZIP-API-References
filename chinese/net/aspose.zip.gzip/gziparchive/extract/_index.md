---
title: GzipArchive.Extract
second_title: Aspose.ZIP for .NET API 参考
description: GzipArchive 方法. 将存档提取到提供的流中
type: docs
weight: 40
url: /zh/net/aspose.zip.gzip/gziparchive/extract/
---
## GzipArchive.Extract method

将存档提取到提供的流中。

```csharp
public void Extract(Stream destination)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| destination | Stream | 目标流。必须是可写的。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentException | *destination*不支持写入。 |

### 例子

```csharp
using (var archive = new GzipArchive("archive.gz"))
{
     archive.Extract(httpResponseStream);
}
```

### 也可以看看

* class [GzipArchive](../)
* 命名空间 [Aspose.Zip.Gzip](../../gziparchive/)
* 部件 [Aspose.Zip](../../../)


