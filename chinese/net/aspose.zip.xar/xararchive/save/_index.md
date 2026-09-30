---
title: "XarArchive.Save"
second_title: "Aspose.ZIP for .NET API 参考"
description: "XarArchive 方法。将存档保存到提供的目标文件"
type: docs
weight: 80
url: /zh/net/aspose.zip.xar/xararchive/save/
---
## Save(string, XarSaveOptions) {#save_1}

将存档保存到提供的目标文件。

```csharp
public void Save(string destinationFileName, XarSaveOptions saveOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationFileName | String | 要创建的归档的路径。如果指定的文件名指向已有文件，将被覆盖。 |
| saveOptions | XarSaveOptions | 用于保存 xar 存档的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *destinationFileName* 为 null。 |
| InvalidOperationException | 无法修改 xar 存档。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| IOException | 打开文件时发生 I/O 错误。 |
| PathTooLongException | 指定的路径、文件名或两者的长度超过系统定义的最大长度。 |
| UnauthorizedAccessException | *destinationFileName* 指定了一个只读文件。 -或- *destinationFileName* 指定了一个目录。 -或- 调用者没有所需的权限。 |

### 另请参阅

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, XarSaveOptions) {#save}

将存档保存到提供的流中。

```csharp
public void Save(Stream output, XarSaveOptions saveOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 输出 | 流 | 目标流。 |
| saveOptions | XarSaveOptions | 用于保存 xar 存档的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *output* 为 null。 |
| ArgumentException | *output*不可写/不可读或不可定位。 |
| InvalidOperationException | 无法修改 xar 存档。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |

### 另请参阅

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


