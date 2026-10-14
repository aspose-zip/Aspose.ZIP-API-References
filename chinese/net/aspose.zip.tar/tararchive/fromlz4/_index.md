---
title: "TarArchive.FromLZ4"
second_title: "Aspose.ZIP for .NET API 参考"
description: "TarArchive 方法。提取提供的 LZ4 归档并从提取的数据组成 TarArchive"
type: docs
weight: 30
url: /zh/net/aspose.zip.tar/tararchive/fromlz4/
---
## FromLZ4(string) {#fromlz4_1}

提取提供的 LZ4 归档并从提取的数据组成 [`TarArchive`](../)。

重要提示：LZ4 归档在此方法中会被完全提取，其内容会保存在内部。请注意内存消耗。

```csharp
public static TarArchive FromLZ4(string path)
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
| SecurityException | 调用者没有访问所需的权限 |
| ArgumentException | 该 *path* 为空，仅包含空白字符，或包含无效字符。 |
| UnauthorizedAccessException | 对文件 *path* 的访问被拒绝。 |
| PathTooLongException | 指定的 *path*、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | *path* 处的文件格式无效。 |
| DirectoryNotFoundException | 指定的路径无效，例如位于未映射的驱动器上。 |
| FileNotFoundException | 未找到该文件。 |
| EndOfStreamException | 该文件太短。 |
| InvalidDataException | 文件的签名不正确。 |
| IOException | 打开文件时发生 I/O 错误。 |
| InvalidOperationException | 已准备好进行组合的归档。 |

## 备注

由于压缩算法的特性，LZ4 提取流不可定位。Tar 归档提供提取任意记录的功能，因此在内部必须使用可定位的流。

### 另请参阅

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZ4(Stream) {#fromlz4}

提取提供的 LZ4 归档并从提取的数据组成 [`TarArchive`](../)。

重要提示：LZ4 归档在此方法中会被完全提取，其内容会保存在内部。请注意内存消耗。

```csharp
public static TarArchive FromLZ4(Stream source)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | 流 | 存档的来源。 |

### Return Value

一个 [`TarArchive`](../) 实例

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentException | 无法从 *source* 读取 |
| ArgumentNullException | *source* 为 null。 |
| EndOfStreamException | *source* 太短。 |
| InvalidDataException | *source* 的签名不正确。 |
| ObjectDisposedException | 如果源流已被释放，则抛出此异常。 |

## 备注

由于压缩算法的特性，LZ4 提取流不可定位。Tar 归档提供提取任意记录的功能，因此在内部必须使用可定位的流。

### 另请参阅

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


