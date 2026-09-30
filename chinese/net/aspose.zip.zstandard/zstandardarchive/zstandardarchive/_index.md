---
title: "ZstandardArchive.ZstandardArchive"
second_title: "Aspose.ZIP for .NET API 参考"
description: "ZstandardArchive 构造函数。初始化一个准备压缩的 ZstandardArchive 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.zip.zstandard/zstandardarchive/zstandardarchive/
---
## ZstandardArchive() {#constructor}

初始化一个准备压缩的 [`ZstandardArchive`](../) 类的新实例。

```csharp
public ZstandardArchive()
```

## 示例

以下示例展示了如何压缩文件。

```csharp
using (ZstandardArchive archive = new ZstandardArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.zst");
}
```

### 另请参阅

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(Stream, ZstandardLoadOptions) {#constructor_1}

初始化一个准备解压的 [`ZstandardArchive`](../) 类的新实例。

```csharp
public ZstandardArchive(Stream sourceStream, ZstandardLoadOptions options = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | 流 | 存档的来源。 |
| 选项 | ZstandardLoadOptions | 用于加载存档的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 如果源流已被释放，则抛出此异常。 |
| EndOfStreamException | 当意外到达流的末尾时抛出此异常。 |
| IOException | 发生 I/O 错误。 |
| InvalidDataException | 当数据无效或损坏时抛出。 |

## 备注

此构造函数不进行解压缩。请参阅 [`Open`](../open/) 方法以进行解压缩。

## 示例

从流中打开存档并将其提取到 `MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new ZstandardArchive(File.OpenRead("archive.zst")))
  archive.Open().CopyTo(ms);
```

### 另请参阅

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(string, ZstandardLoadOptions) {#constructor_2}

初始化一个 [`ZstandardArchive`](../) 类的新实例。

```csharp
public ZstandardArchive(string path, ZstandardLoadOptions options = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | 存档文件的路径。 |
| 选项 | ZstandardLoadOptions | 用于加载存档的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *path* 为 null。 |
| SecurityException | 调用方没有访问所需的权限。 |
| ArgumentException | 该 *path* 为空，仅包含空白字符，或包含无效字符。 |
| UnauthorizedAccessException | 对文件 *path* 的访问被拒绝。 |
| PathTooLongException | 指定的 *path*、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 位于 *path* 的文件在字符串中间包含冒号 (:)。 |
| DirectoryNotFoundException | 指定的路径无效，例如位于未映射的驱动器上。 |
| EndOfStreamException | 当意外到达流的末尾时抛出此异常。 |
| FileNotFoundException | 未找到该文件。 |
| IOException | 该文件已打开。 |
| InvalidDataException | 当数据无效或损坏时抛出。 |

## 备注

此构造函数不进行解压缩。请参阅 [`Open`](../open/) 方法以进行解压缩。

## 示例

通过路径从文件打开存档并将其提取到 `MemoryStream`

```csharp
var ms = new MemoryStream();
using (ZstandardArchive archive = new ZstandardArchive("archive.zst"))
  archive.Open().CopyTo(ms);
```

### 另请参阅

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


