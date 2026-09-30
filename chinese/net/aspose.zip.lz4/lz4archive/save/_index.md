---
title: "Lz4Archive.Save"
second_title: "Aspose.ZIP for .NET API 参考"
description: "Lz4Archive 方法。将 lz4 存档保存到提供的流中"
type: docs
weight: 60
url: /zh/net/aspose.zip.lz4/lz4archive/save/
---
## Save(Stream) {#save_1}

将 lz4 存档保存到提供的流。

```csharp
public void Save(Stream output)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 输出 | 流 | 目标流。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *output* 为 null。 |
| ArgumentException | *output* 不可写。 |
| InvalidOperationException | 存档已准备好进行提取。 - 或者 - 未提供源。 |
| OperationCanceledException | 在 .NET Framework 4.0 及以上版本：当通过提供的取消令牌取消压缩时抛出。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |

## 备注

*output* must be seekable.

## 示例

```csharp
using (FileStream lz4File = File.Open("archive.lz4", FileMode.Create))
{
    using (var archive = new Lz4Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(lz4File);
     }
}
```

### 另请参阅

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

将 lz4 存档保存到提供的目标文件。

```csharp
public void Save(FileInfo destination)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目标 | FileInfo | FileInfo，将作为目标流打开。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| SecurityException | 调用者没有打开 *destination* 所需的权限。 |
| ArgumentException | 文件路径为空或仅包含空白字符。 |
| FileNotFoundException | 未找到该文件。 |
| UnauthorizedAccessException | 文件路径为只读或是目录。 |
| ArgumentNullException | *destination* 为 null。 |
| DirectoryNotFoundException | 指定的路径无效，例如位于未映射的驱动器上。 |
| IOException | 该文件已打开。 |
| InvalidOperationException | 已准备好进行提取的归档。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |

## 示例

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz4"));
}
```

### 另请参阅

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

将存档保存到提供的目标文件。

```csharp
public void Save(string destinationFileName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationFileName | String | 要创建的归档的路径。如果指定的文件名指向已有文件，将被覆盖。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *destinationFileName* 为 null。 |
| SecurityException | 调用者没有访问所需的权限 |
| ArgumentException | *destinationFileName* 为空，仅包含空白字符，或包含无效字符。 |
| UnauthorizedAccessException | 对文件 *destinationFileName* 的访问被拒绝。 |
| PathTooLongException | 指定的 *destinationFileName*、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须小于 248 个字符，文件名必须小于 260 个字符。 |
| NotSupportedException | 位于 *destinationFileName* 的文件在字符串中间包含冒号 (:)。 |
| InvalidOperationException | 已准备好进行提取的归档。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| DirectoryNotFoundException | 指定的路径无效，（例如，它位于未映射的驱动器上）。 |
| FileNotFoundException | 在 *destinationFileName* 中指定的文件未找到。 |
| IOException | 打开文件时发生 I/O 错误。 |

## 示例

```csharp
using (var archive = new LZ4Archive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### 另请参阅

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


