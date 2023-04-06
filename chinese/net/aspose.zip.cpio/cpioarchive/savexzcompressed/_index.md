---
title: CpioArchive.SaveXzCompressed
second_title: Aspose.ZIP for .NET API 参考
description: CpioArchive 方法. 使用 xz 压缩将存档保存到流中
type: docs
weight: 100
url: /zh/net/aspose.zip.cpio/cpioarchive/savexzcompressed/
---
## SaveXzCompressed(Stream, CpioFormat, XzArchiveSettings) {#savexzcompressed}

使用 xz 压缩将存档保存到流中。

```csharp
public void SaveXzCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| output | Stream | 目标流。 |
| cpioFormat | CpioFormat | 定义 cpio 标头格式。 |
| settings | XzArchiveSettings | 一组设置特定的 xz 存档：字典大小、块大小、检查类型。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *output*一片空白。 |
| ArgumentException | *output*不可写。 |

### 评论

*output*流必须是可写的。

### 例子

```csharp
using (FileStream result = File.OpenWrite("result.cpio.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### 也可以看看

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* 命名空间 [Aspose.Zip.Cpio](../../cpioarchive/)
* 部件 [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, CpioFormat, XzArchiveSettings) {#savexzcompressed_1}

将压缩包按路径保存到 xz 压缩路径下。

```csharp
public void SaveXzCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| path | String | 要创建的存档的路径。如果指定的文件名指向一个现有文件，它将被覆盖。 |
| cpioFormat | CpioFormat | 定义 cpio 标头格式。 |
| settings | XzArchiveSettings | 一组设置特定的 xz 存档：字典大小、块大小、检查类型。 |

### 例子

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.cpio.xz");
    }
}
```

### 也可以看看

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* 命名空间 [Aspose.Zip.Cpio](../../cpioarchive/)
* 部件 [Aspose.Zip](../../../)


