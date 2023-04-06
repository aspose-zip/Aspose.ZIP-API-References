---
title: RarArchive.RarArchive
second_title: Aspose.ZIP for .NET API 参考
description: RarArchive 构造函数. 初始化一个新的实例RarArchive可以从存档中提取类和组合条目列表
type: docs
weight: 10
url: /zh/net/aspose.zip.rar/rararchive/rararchive/
---
## RarArchive(string, RarArchiveLoadOptions) {#constructor_1}

初始化一个新的实例[`RarArchive`](../)可以从存档中提取类和组合条目列表。

```csharp
public RarArchive(string path, RarArchiveLoadOptions loadOptions = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| path | String | 存档文件的完全限定路径或相对路径。 |
| loadOptions | RarArchiveLoadOptions | 加载现有存档的选项。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *path*一片空白。 |
| SecurityException | 调用者没有所需的访问权限。 |
| ArgumentException | 这*path*为空、仅包含空格或包含无效字符。 |
| UnauthorizedAccessException | 访问文件*path*被拒绝。 |
| PathTooLongException | 指定的*path*、文件名或两者都超过了系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 归档于*path*在字符串中间包含一个冒号 (:)。 |

### 评论

此构造函数不解压缩任何条目。看[`Open`](../../rararchiveentry/open/)解压方法.

### 例子

以下示例提取存档，然后将第一个条目解压缩到`内存流`.

```csharp
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive("data.rar"))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### 也可以看看

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* 命名空间 [Aspose.Zip.Rar](../../rararchive/)
* 部件 [Aspose.Zip](../../../)

---

## RarArchive(Stream, RarArchiveLoadOptions) {#constructor}

初始化一个新的实例[`RarArchive`](../)可以从存档中提取类和组合条目列表。

```csharp
public RarArchive(Stream sourceStream, RarArchiveLoadOptions loadOptions = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | Stream | 存档的来源。 |
| loadOptions | RarArchiveLoadOptions | 加载现有存档的选项。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentException | *sourceStream*不可搜索。 |
| InvalidDataException | 存档签名错误。 - 或 - 该文件不是 RAR 压缩文件。 |
| InvalidOperationException |  |

### 评论

此构造函数不解压缩任何条目。看[`Open`](../../rararchiveentry/open/)解压方法.

### 例子

以下示例解密并解压缩第一个条目`内存流`.

```csharp
var fs = File.OpenRead("encrypted.rar");
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive(fs, new RarArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### 也可以看看

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* 命名空间 [Aspose.Zip.Rar](../../rararchive/)
* 部件 [Aspose.Zip](../../../)


