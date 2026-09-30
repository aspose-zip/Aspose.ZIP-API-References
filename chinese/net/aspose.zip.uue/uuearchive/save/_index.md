---
title: "UueArchive.Save"
second_title: "Aspose.ZIP for .NET API 参考"
description: "UueArchive 方法。将归档保存到提供的流中"
type: docs
weight: 70
url: /zh/net/aspose.zip.uue/uuearchive/save/
---
## Save(Stream, UueSaveOptions) {#save}

将存档保存到提供的流中。

```csharp
public void Save(Stream outputStream, UueSaveOptions saveOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| outputStream | 流 | 目标流。 |
| saveOptions | UueSaveOptions | 归档保存的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| InvalidOperationException | 未提供要归档的数据源。 |
| ArgumentException | *outputStream* 不可写。 |
| UnauthorizedAccessException | 文件源是只读的或是一个目录。 |
| DirectoryNotFoundException | 指定的文件源路径无效，例如位于未映射的驱动器上。 |
| IOException | 文件源已打开。 |

## 备注

*outputStream* must be writable.

## 示例

将压缩数据写入 http 响应流。

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### 另请参阅

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, UueSaveOptions) {#save_1}

将存档保存到提供的目标文件中。

```csharp
public void Save(string destinationFileName, UueSaveOptions saveOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationFileName | String | 要创建的归档的路径。如果指定的文件名指向已有文件，将被覆盖。 |
| saveOptions | UueSaveOptions | 归档保存的选项。 |

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
| InvalidOperationException | 未提供要归档的数据源。 |

## 示例

将编码数据写入文件。

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.uue");
}
```

### 另请参阅

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


