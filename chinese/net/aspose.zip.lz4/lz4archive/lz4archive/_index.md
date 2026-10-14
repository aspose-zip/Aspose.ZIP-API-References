---
title: "Lz4Archive.Lz4Archive"
second_title: "Aspose.ZIP for .NET API 参考"
description: "Lz4Archive 构造函数。初始化一个为解压缩准备好的 Lz4Archive 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.zip.lz4/lz4archive/lz4archive/
---
## Lz4Archive(Stream, Lz4LoadOptions) {#constructor_1}

初始化一个为解压缩准备好的 [`Lz4Archive`](../) 类的新实例。

```csharp
public Lz4Archive(Stream sourceStream, Lz4LoadOptions loadOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | 流 | 存档的来源。 |
| loadOptions | Lz4LoadOptions | 用于加载存档的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentException | 无法从 *sourceStream* 读取 |
| ArgumentNullException | *sourceStream* 为 null。 |
| EndOfStreamException | *sourceStream* 太短。 |
| InvalidDataException | *sourceStream* 的签名错误。 |
| ObjectDisposedException | 如果源流已被释放，则抛出此异常。 |
| IOException | 发生 I/O 错误。 |

## 备注

此构造函数不进行解压缩。请参阅 [`Open`](../open/) 方法以进行解压缩。

## 示例

从流中打开存档并将其提取到 `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive(File.OpenRead("archive.lz4")))
  archive.Open().CopyTo(ms);
```

### 另请参阅

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(string, Lz4LoadOptions) {#constructor_2}

初始化一个 [`Lz4Archive`](../) 类的新实例。

```csharp
public Lz4Archive(string path, Lz4LoadOptions loadOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | 存档文件的路径。 |
| loadOptions | Lz4LoadOptions | 用于加载存档的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *path* 为 null。 |
| SecurityException | 调用者没有访问所需的权限 |
| ArgumentException | 该 *path* 为空，仅包含空白字符，或包含无效字符。 |
| UnauthorizedAccessException | 对文件 *path* 的访问被拒绝。 |
| PathTooLongException | 指定的 *path*、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 位于 *path* 的文件在字符串中间包含冒号 (:)。 |
| EndOfStreamException | 该文件太短。 |
| InvalidDataException | 文件中的数据签名错误。 |
| DirectoryNotFoundException | 指定的路径无效，例如位于未映射的驱动器上。 |
| FileNotFoundException | 未找到该文件。 |
| IOException | 该文件已打开。 |

## 备注

此构造函数不进行解压缩。请参阅 [`Open`](../open/) 方法以进行解压缩。

## 示例

通过路径从文件打开存档并将其提取到 `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive("archive.lz4"))
  archive.Open().CopyTo(ms);
```

### 另请参阅

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(Lz4ArchiveSetting) {#constructor}

初始化一个为压缩准备好的 [`Lz4Archive`](../) 类的新实例。

```csharp
public Lz4Archive(Lz4ArchiveSetting settings = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 设置 | Lz4ArchiveSetting | 复合归档的设置。 |

### 另请参阅

* class [Lz4ArchiveSetting](../../lz4archivesetting/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


