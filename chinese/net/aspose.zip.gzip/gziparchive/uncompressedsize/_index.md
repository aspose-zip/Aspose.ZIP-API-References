---
title: "GzipArchive.UncompressedSize"
second_title: "Aspose.ZIP for .NET API 参考"
description: "GzipArchive 属性。获取原始文件的大小"
type: docs
weight: 30
url: /zh/net/aspose.zip.gzip/gziparchive/uncompressedsize/
---
## GzipArchive.UncompressedSize property

获取原始文件的大小。

```csharp
public ulong UncompressedSize { get; }
```

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放，无法使用。 |

## 备注

在解压缩期间，此属性可能包含不正确的大小。如果未压缩文件大小超过 4GB，由于标题中的 32 位限制，此属性将给出错误的值。

### 另请参阅

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


