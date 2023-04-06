---
title: TarArchive.SaveZCompressed
second_title: Aspose.ZIP for .NET API 参考
description: TarArchive 方法. 使用 Z 压缩将存档保存到流中
type: docs
weight: 160
url: /zh/net/aspose.zip.tar/tararchive/savezcompressed/
---
## SaveZCompressed(Stream, TarFormat?) {#savezcompressed}

使用 Z 压缩将存档保存到流中。

```csharp
public void SaveZCompressed(Stream output, TarFormat? format = default)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| output | Stream | 目标流。 |
| format | Nullable`1 | 定义 tar 标头格式。在可能的情况下，空值将被视为 USTAr。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *output*一片空白。 |
| ArgumentException | *output*不可写。 |

### 评论

*output*必须是可写的。

### 例子

```csharp
using (FileStream result = File.OpenWrite("result.tar.Z"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZCompressed(result);
        }
    }
}
```

### 也可以看看

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* 命名空间 [Aspose.Zip.Tar](../../tararchive/)
* 部件 [Aspose.Zip](../../../)

---

## SaveZCompressed(string, TarFormat?) {#savezcompressed_1}

以Z压缩的方式将压缩包保存到路径中。

```csharp
public void SaveZCompressed(string path, TarFormat? format = default)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| path | String | 要创建的存档的路径。如果指定的文件名指向一个现有文件，它将被覆盖。 |
| format | Nullable`1 | 定义 tar 标头格式。在可能的情况下，空值将被视为 USTAr。 |

### 例子

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZCompressed("result.tar.Z");
    }
}
```

### 也可以看看

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* 命名空间 [Aspose.Zip.Tar](../../tararchive/)
* 部件 [Aspose.Zip](../../../)


