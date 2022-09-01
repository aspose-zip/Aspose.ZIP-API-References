---
title: FromGZip
second_title: Aspose.ZIP for .NET API 参考
description: 提取提供的 gzip 存档并从提取的数据中组成TarArchiveaspose.zip.tar/tararchive
type: docs
weight: 20
url: /zh/net/aspose.zip.tar/tararchive/fromgzip/
---
## FromGZip(Stream) {#fromgzip}

提取提供的 gzip 存档并从提取的数据中组成[`TarArchive`](../../tararchive)。

重要提示：gzip 存档在此方法中完全提取，其内容保存在内部。小心内存消耗。

```csharp
public static TarArchive FromGZip(Stream source)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| source | Stream | 存档的来源。 |

### 返回值

[`TarArchive`](../../tararchive)

### 评论

GZip 提取流的实例不可被压缩算法的本质。 Tar 存档提供了提取任意记录的工具，因此它必须在引擎盖下操作可搜索的流。

### 也可以看看

* class [TarArchive](../../tararchive)
* 命名空间 [Aspose.Zip.Tar](../../tararchive)
* 部件 [Aspose.Zip](../../../)

---

## FromGZip(string) {#fromgzip_1}

提取提供的 gzip 存档并从提取的数据中组成[`TarArchive`](../../tararchive)。

重要提示：gzip 存档在此方法中完全提取，其内容保存在内部。小心内存消耗。

```csharp
public static TarArchive FromGZip(string path)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| path | String | 存档文件的路径。 |

### 返回值

[`TarArchive`](../../tararchive)

### 评论

GZip 提取流的实例不可被压缩算法的本质。 Tar 存档提供了提取任意记录的工具，因此它必须在引擎盖下操作可搜索的流。

### 也可以看看

* class [TarArchive](../../tararchive)
* 命名空间 [Aspose.Zip.Tar](../../tararchive)
* 部件 [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->