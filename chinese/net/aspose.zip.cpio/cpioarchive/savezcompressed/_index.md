---
title: "CpioArchive.SaveZCompressed"
second_title: "Aspose.ZIP for .NET API 参考"
description: "CpioArchive 方法。使用 Z 压缩将存档保存到流中。"
type: docs
weight: 130
url: /zh/net/aspose.zip.cpio/cpioarchive/savezcompressed/
---
## SaveZCompressed(Stream, CpioFormat) {#savezcompressed}

使用 Z 压缩将存档保存到流中。

```csharp
public void SaveZCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
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
using (FileStream result = File.OpenWrite("result.cpio.Z"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZCompressed(result);
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

## SaveZCompressed(string, CpioFormat) {#savezcompressed_1}

使用 Z 压缩将存档按路径保存到指定路径。

```csharp
public void SaveZCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | 要创建的归档的路径。如果指定的文件名指向已有文件，将被覆盖。 |
| cpioFormat | CpioFormat | 定义 cpio 头部格式。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| ArgumentNullException | *path* 为 `null`。 |
| DirectoryNotFoundException | 指定的路径无效，（例如，它位于未映射的驱动器上）。 |
| IOException | 发生 I/O 错误。 |
| PathTooLongException | 指定的路径、文件名或两者的长度超过系统定义的最大长度。 |

## 示例

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZCompressed("result.cpio.Z");
    }
}
```

### 另请参阅

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


