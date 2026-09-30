---
title: "CabArchive.Save"
second_title: "Aspose.ZIP for .NET API 参考"
description: "CabArchive 方法。将存档保存到提供的流中"
type: docs
weight: 70
url: /zh/net/aspose.zip.cab/cabarchive/save/
---
## Save(Stream, CabSaveOptions) {#save}

将存档保存到提供的流中。

```csharp
public void Save(Stream outputStream, CabSaveOptions saveOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| outputStream | 流 | 目标流。 |
| saveOptions | CabSaveOptions | 存档保存的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentException | *outputStream* 不可写且不可定位。 |
| ObjectDisposedException | 存档已释放。 |
| InvalidOperationException | 存档已准备好进行提取，无法保存。 |

## 备注

*outputStream* must be writable.

## 示例

```csharp
using (FileStream cabFile = File.Open("archive.cab", FileMode.Create))
{
    using (var archive = new CabArchive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(cabFile);
    }
}
```

### 另请参阅

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, CabSaveOptions) {#save_1}

将存档保存到提供的目标文件。

```csharp
public void Save(string destinationFileName, CabSaveOptions saveOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationFileName | String | 要创建的归档的路径。如果指定的文件名指向已有文件，将被覆盖。 |
| saveOptions | CabSaveOptions | 存档保存的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *destinationFileName* 为 null。 |
| SecurityException | 调用方没有访问所需的权限。 |
| ArgumentException | *destinationFileName* 为空，仅包含空白字符，或包含无效字符。 |
| UnauthorizedAccessException | 对文件 *destinationFileName* 的访问被拒绝。 |
| PathTooLongException | 指定的 *destinationFileName*、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须小于 248 个字符，文件名必须小于 260 个字符。 |
| NotSupportedException | 位于 *destinationFileName* 的文件在字符串中间包含冒号 (:)。 |
| FileNotFoundException | 未找到该文件。 |
| InvalidOperationException | 存档已打开用于提取。 |
| DirectoryNotFoundException | 指定的路径无效，例如位于未映射的驱动器上。 |
| IOException | 该文件已打开。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |

## 备注

可以将存档保存到其加载的相同路径。但不推荐这样做，因为此方法会复制到临时文件。

## 示例

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### 另请参阅

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


