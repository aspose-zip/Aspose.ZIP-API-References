---
title: "TarArchive.SaveLZ4Compressed"
second_title: "Aspose.ZIP for .NET API 参考"
description: "TarArchive 方法。使用 LZ4 压缩将归档保存到流中"
type: docs
weight: 170
url: /zh/net/aspose.zip.tar/tararchive/savelz4compressed/
---
## SaveLZ4Compressed(Stream, TarFormat?) {#savelz4compressed}

使用 LZ4 压缩将归档保存到流中。

```csharp
public void SaveLZ4Compressed(Stream output, TarFormat? format = default)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 输出 | 流 | 目标流。 |
| 格式 | Nullable`1 | 定义 tar 头部格式。空值将在可能时被视为 USTar。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *output* 为 null。 |
| ArgumentException | *output* 不可写。 |
| ObjectDisposedException | 存档已被释放，无法使用 |
| IOException | 发生 I/O 错误。 |

## 备注

*output* must be writable.

## 示例

```csharp
using (FileStream result = File.OpenWrite("result.tar.lz4"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZ4Compressed(result);
        }
    }
}
```

### 另请参阅

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLZ4Compressed(string, TarFormat?) {#savelz4compressed_1}

使用 LZ4 压缩将归档保存到指定路径的文件中。

```csharp
public void SaveLZ4Compressed(string path, TarFormat? format = default)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | 要创建的归档的路径。如果指定的文件名指向已有文件，将被覆盖。 |
| 格式 | Nullable`1 | 定义 tar 头部格式。空值将在可能时被视为 USTar。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| UnauthorizedAccessException | 调用者没有所需的权限。-或- *path* 指定了只读文件或目录。 |
| ArgumentException | *path* 是长度为零的字符串，仅包含空白，或包含由 InvalidPathChars 定义的一个或多个无效字符。 |
| ArgumentNullException | *path* 为 null。 |
| PathTooLongException | 指定的 *path*、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| DirectoryNotFoundException | 指定的 *path* 无效（例如，它位于未映射的驱动器上）。 |
| NotSupportedException | *path* 的格式无效。 |
| ObjectDisposedException | 存档已被释放，无法使用 |
| IOException | 发生 I/O 错误。 |

## 示例

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZ4Compressed("result.tar.lz4");
    }
}
```

### 另请参阅

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


