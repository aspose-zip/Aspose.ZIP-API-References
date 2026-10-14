---
title: "TarArchive.FromLZMA"
second_title: "Aspose.ZIP for .NET API 参考"
description: "TarArchive 方法。提取提供的 LZMA 存档并根据提取的数据组成 TarArchive。"
type: docs
weight: 50
url: /zh/net/aspose.zip.tar/tararchive/fromlzma/
---
## FromLZMA(Stream) {#fromlzma}

提取提供的 LZMA 存档并根据提取的数据组成 [`TarArchive`](../)。

重要提示：LZMA 存档在此方法中被完整提取，其内容在内部保留。请注意内存消耗。

```csharp
public static TarArchive FromLZMA(Stream source)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | 流 | 存档的来源。 |

### Return Value

一个 [`TarArchive`](../) 实例

### 异常

| 异常 | 条件 |
| --- | --- |
| InvalidDataException | 存档已损坏。 |
| EndOfStreamException | 当在读取预期的字节数之前到达流的末尾时抛出此异常。 |
| ObjectDisposedException | 如果源流已被释放，则抛出此异常。 |
| ArgumentNullException | *source* 为 null。 |
| IOException | 发生 I/O 错误。 |

## 备注

由于压缩算法的特性，LZMA 提取流不可定位。Tar 存档提供提取任意记录的功能，因此在底层必须使用可定位的流。

### 另请参阅

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZMA(string) {#fromlzma_1}

提取提供的 LZMA 存档并根据提取的数据组成 [`TarArchive`](../)。

重要提示：LZMA 存档在此方法中被完整提取，其内容在内部保留。请注意内存消耗。

```csharp
public static TarArchive FromLZMA(string path)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | 存档文件的路径。 |

### Return Value

一个 [`TarArchive`](../) 实例

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *path* 为 null。 |
| ArgumentException | 该 *path* 为空，仅包含空白字符，或包含无效字符。 |
| UnauthorizedAccessException | 对文件 *path* 的访问被拒绝。 |
| PathTooLongException | 指定的 *path*、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | *path* 处的文件格式无效。 |
| DirectoryNotFoundException | 指定的路径无效，例如位于未映射的驱动器上。 |
| FileNotFoundException | 未找到该文件。 |
| EndOfStreamException | 当在读取预期的字节数之前到达流的末尾时抛出此异常。 |
| IOException | 打开文件时发生 I/O 错误。 |
| InvalidDataException | 存档已损坏。 |

## 备注

由于压缩算法的特性，LZMA 提取流不可定位。Tar 存档提供提取任意记录的功能，因此在底层必须使用可定位的流。

### 另请参阅

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


