---
title: "IsoArchive.Save"
second_title: "Aspose.ZIP for .NET API 参考"
description: "IsoArchive 方法。将 ISO 映像保存到指定路径。"
type: docs
weight: 70
url: /zh/net/aspose.zip.iso/isoarchive/save/
---
## Save(string, IsoSaveOptions) {#save_1}

将 ISO 镜像保存到指定路径。

```csharp
public void Save(string path, IsoSaveOptions saveOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | ISO 映像将被保存的路径。 |
| saveOptions | IsoSaveOptions | 用于保存 ISO 存档的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| InvalidOperationException | 当存档未处于编辑模式时抛出。 |
| ArgumentNullException | 当 *path* 为 null 时抛出。 |
| DirectoryNotFoundException | 当指定的路径无效时抛出，例如位于未映射的驱动器上。 |
| IOException | 当文件已打开时抛出。 |
| UnauthorizedAccessException | 当对文件 *path* 的访问被拒绝时抛出。 |
| PathTooLongException | 当指定的 *path* 超过系统定义的最大长度时抛出。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |

## 示例

以下示例展示了如何将 ISO 存档保存到文件：

```csharp
// 创建一个新的空 ISO 存档
using(IsoArchive isoArchive = new IsoArchive())
{
    // 向 ISO 存档添加文件
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // 将 ISO 存档保存到文件
    isoArchive.Save("new_archive.iso");
}
```

### 另请参阅

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, IsoSaveOptions) {#save}

将 ISO 镜像保存到指定的流。

```csharp
public void Save(Stream stream, IsoSaveOptions saveOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | ISO 映像将被保存的流。 |
| saveOptions | IsoSaveOptions | 用于保存 ISO 存档的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| InvalidOperationException | 当存档未处于编辑模式时抛出。 |
| ArgumentNullException | 当 *stream* 为 null 时抛出。 |
| ArgumentException | 当 *stream* 不可写入时抛出。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| IOException | 发生 I/O 错误。 |

## 示例

下面的示例展示了如何将 ISO 存档保存到内存流：

```csharp

 // 创建一个新的空 ISO 存档
 using(IsoArchive isoArchive = new IsoArchive())
 {
     // 向 ISO 存档添加文件
     isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

     // 将 ISO 存档保存到内存流
     isoArchive.Save(memoryStream);
 }
```

### 另请参阅

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


