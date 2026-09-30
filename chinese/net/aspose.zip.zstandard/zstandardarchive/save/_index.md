---
title: "ZstandardArchive.Save"
second_title: "Aspose.ZIP for .NET API 参考"
description: "ZstandardArchive 方法。将存档保存到提供的流中"
type: docs
weight: 60
url: /zh/net/aspose.zip.zstandard/zstandardarchive/save/
---
## Save(Stream, ZstandardSaveOptions) {#save_1}

将存档保存到提供的流中。

```csharp
public void Save(Stream outputStream, ZstandardSaveOptions settings = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| outputStream | 流 | 目标流。 |
| 设置 | ZstandardSaveOptions | 用于存档组成的可选设置。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| ArgumentException | *outputStream* 不可写。 |
| InvalidOperationException | 未提供源。 |

## 备注

*outputStream* must be writable.

## 示例

将压缩数据写入 http 响应流。

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### 另请参阅

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, ZstandardSaveOptions) {#save_2}

将存档保存到提供的目标文件。

```csharp
public void Save(string destinationFileName, ZstandardSaveOptions settings = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationFileName | String | 要创建的归档的路径。如果指定的文件名指向已有文件，将被覆盖。 |
| 设置 | ZstandardSaveOptions | 用于存档组成的可选设置。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| ArgumentNullException | *destinationFileName* 为 null。 |
| SecurityException | 调用方没有访问所需的权限。 |
| ArgumentException | *destinationFileName* 为空，仅包含空白字符，或包含无效字符。 |
| UnauthorizedAccessException | 对文件 *destinationFileName* 的访问被拒绝。 |
| PathTooLongException | 指定的 *destinationFileName*、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须小于 248 个字符，文件名必须小于 260 个字符。 |
| NotSupportedException | 位于 *destinationFileName* 的文件在字符串中间包含冒号 (:)。 |
| 异常 | 当运行时错误发生时抛出。 |
| DirectoryNotFoundException | 指定的路径无效，（例如，它位于未映射的驱动器上）。 |
| IOException | 打开文件时发生 I/O 错误。 |
| InvalidOperationException | 未提供源。 |

## 示例

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.zst");
}
```

### 另请参阅

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo, ZstandardSaveOptions) {#save}

将存档保存到提供的目标文件。

```csharp
public void Save(FileInfo destination, ZstandardSaveOptions settings = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目标 | FileInfo | FileInfo，将作为目标流打开。 |
| 设置 | ZstandardSaveOptions | 用于存档组成的可选设置。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| SecurityException | 调用者没有打开 *destination* 所需的权限。 |
| ArgumentException | 文件路径为空或仅包含空白字符。 |
| FileNotFoundException | 未找到该文件。 |
| UnauthorizedAccessException | 文件路径为只读或是目录。 |
| ArgumentNullException | *destination* 为 null。 |
| DirectoryNotFoundException | 指定的路径无效，例如位于未映射的驱动器上。 |
| IOException | 该文件已打开。 |
| InvalidOperationException | 未提供源。 |

## 示例

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.zst"));
}
```

### 另请参阅

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


