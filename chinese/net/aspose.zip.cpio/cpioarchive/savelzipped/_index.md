---
title: "CpioArchive.SaveLzipped"
second_title: "Aspose.ZIP for .NET API 参考"
description: "CpioArchive 方法。使用 lzip 压缩将存档保存到流中"
type: docs
weight: 100
url: /zh/net/aspose.zip.cpio/cpioarchive/savelzipped/
---
## SaveLzipped(Stream, CpioFormat) {#savelzipped}

使用 lzip 压缩将存档保存到流中。

```csharp
public void SaveLzipped(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 输出 | 流 | 目标流。 |
| cpioFormat | CpioFormat | 定义 cpio 头部格式。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *output* 为 null。 |
| ArgumentException | *output* 不可写。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |

## 备注

*output* must be writable.

## 示例

```csharp
using (FileStream result = File.OpenWrite("result.cpio.lz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
        }
    }
}
```

### 另请参阅

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLzipped(string, CpioFormat) {#savelzipped_1}

使用 lzip 压缩将存档保存到指定路径的文件中。

```csharp
public void SaveLzipped(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | 要创建的归档的路径。如果指定的文件名指向已有文件，将被覆盖。 |
| cpioFormat | CpioFormat | 定义 cpio 头部格式。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| ArgumentException | *path* 是长度为零的字符串，仅包含空白，或包含由 InvalidPathChars 定义的一个或多个无效字符。 |
| ArgumentNullException | *path* 为 `null`。 |
| DirectoryNotFoundException | 指定的路径无效，（例如，它位于未映射的驱动器上）。 |
| IOException | 发生 I/O 错误。 |
| PathTooLongException | 指定的路径、文件名或两者的长度超过系统定义的最大长度。 |
| UnauthorizedAccessException | 调用者没有所需的权限。-或- *path* 指定了只读文件或目录。 |

## 示例

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.cpio.lz");
    }
}
```

### 另请参阅

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


