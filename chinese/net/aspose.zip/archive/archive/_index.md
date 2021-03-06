---
title: Archive
second_title: Aspose.ZIP for .NET API 参考
description: 使用其条目的可选设置初始化Archiveaspose.zip/archive类的新实例
type: docs
weight: 10
url: /zh/net/aspose.zip/archive/archive/
---
## Archive(ArchiveEntrySettings) {#constructor}

使用其条目的可选设置初始化[`Archive`](../../archive)类的新实例。

```csharp
public Archive(ArchiveEntrySettings newEntrySettings = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| newEntrySettings | ArchiveEntrySettings | 用于新添加的[`ArchiveEntry`](../../archiveentry)项目的压缩和加密设置。 如果未指定，将使用最常见的 Deflate 压缩而不加密。 |

### 例子

以下示例显示如何使用默认设置压缩单个文件。

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### 也可以看看

* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* 命名空间 [Aspose.Zip](../../archive)
* 部件 [Aspose.Zip](../../../)

---

## Archive(Stream, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_1}

初始化[`Archive`](../../archive)类的新实例并组成条目列表可以从存档中提取。

```csharp
public Archive(Stream sourceStream, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | Stream | 存档的来源。 |
| loadOptions | ArchiveLoadOptions | 加载现有存档的选项。 |
| newEntrySettings | ArchiveEntrySettings | 用于新添加的[`ArchiveEntry`](../../archiveentry)项目的压缩和加密设置。 如果未指定，将使用最常见的 Deflate 压缩而不加密。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentException | *sourceStream*不可搜索。 |
| InvalidDataException | AES 的加密标头与 WinZip 压缩方法相矛盾。 |

### 评论

此构造函数不解压缩任何条目。请参阅[`Open`](../../archiveentry/open)解压方法。

### 例子

以下示例提取加密存档，然后将第一个条目解压缩到` MemoryStream` 。

```csharp
var fs = File.OpenRead("encrypted.zip");
var extracted = new MemoryStream();
using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

* class [ArchiveLoadOptions](../../archiveloadoptions)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* 命名空间 [Aspose.Zip](../../archive)
* 部件 [Aspose.Zip](../../../)

---

## Archive(string, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_2}

初始化[`Archive`](../../archive)类的新实例并组成条目列表可以从存档中提取。

```csharp
public Archive(string path, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| path | String | 归档文件的完全限定或相对路径。 |
| loadOptions | ArchiveLoadOptions | 加载现有存档的选项。 |
| newEntrySettings | ArchiveEntrySettings | 用于新添加的[`ArchiveEntry`](../../archiveentry)项目的压缩和加密设置。 如果未指定，将使用最常见的 Deflate 压缩而不加密。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *path*为空。 |
| SecurityException | 调用者没有访问所需的权限 |
| ArgumentException | *path*为空，仅包含空格，或包含无效字符。 |
| UnauthorizedAccessException | 对文件*path*的访问被拒绝。 |
| PathTooLongException | 指定的*path*、文件名或两者都超过了系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | *path*的文件在字符串中间包含一个冒号 (:)。 |

### 评论

此构造函数不解压缩任何条目。请参阅[`Open`](../../archiveentry/open)解压方法。

### 例子

以下示例提取加密存档，然后将第一个条目解压缩到` MemoryStream` 。

```csharp
var extracted = new MemoryStream();
using (Archive archive = new Archive("encrypted.zip", new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

* class [ArchiveLoadOptions](../../archiveloadoptions)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* 命名空间 [Aspose.Zip](../../archive)
* 部件 [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
