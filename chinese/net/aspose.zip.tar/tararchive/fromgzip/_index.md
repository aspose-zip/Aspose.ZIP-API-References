---
title: TarArchive.FromGZip
second_title: Aspose.ZIP for .NET API 参考
description: TarArchive 方法. 提取提供的 gzip 存档并撰写TarArchive从提取的数据.
type: docs
weight: 20
url: /zh/net/aspose.zip.tar/tararchive/fromgzip/
---
## FromGZip(Stream) {#fromgzip}

提取提供的 gzip 存档并撰写[`TarArchive`](../)从提取的数据.

重要提示：gzip 存档在此方法中完全提取，其内容保留在内部。当心内存消耗.

```csharp
public static TarArchive FromGZip(Stream source)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| source | Stream | 存档的来源。 |

### 返回值

的实例[`TarArchive`](../)

### 评论

GZip 提取流根据压缩算法的性质是不可搜索的。 Tar 存档提供了提取任意记录的工具，因此它必须在幕后操作可搜索流。

### 也可以看看

* class [TarArchive](../)
* 命名空间 [Aspose.Zip.Tar](../../tararchive/)
* 部件 [Aspose.Zip](../../../)

---

## FromGZip(string) {#fromgzip_1}

提取提供的 gzip 存档并撰写[`TarArchive`](../)从提取的数据.

重要提示：gzip 存档在此方法中完全提取，其内容保留在内部。当心内存消耗.

```csharp
public static TarArchive FromGZip(string path)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| path | String | 存档文件的路径。 |

### 返回值

的实例[`TarArchive`](../)

### 评论

GZip 提取流根据压缩算法的性质是不可搜索的。 Tar 存档提供了提取任意记录的工具，因此它必须在幕后操作可搜索流。

### 也可以看看

* class [TarArchive](../)
* 命名空间 [Aspose.Zip.Tar](../../tararchive/)
* 部件 [Aspose.Zip](../../../)


