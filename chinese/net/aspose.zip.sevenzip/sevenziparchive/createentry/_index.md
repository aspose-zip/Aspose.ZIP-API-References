---
title: CreateEntry
second_title: Aspose.ZIP for .NET API 参考
description: 在存档中创建单个条目
type: docs
weight: 50
url: /zh/net/aspose.zip.sevenzip/sevenziparchive/createentry/
---
## CreateEntry(string, FileInfo, bool, SevenZipEntrySettings) {#createentry}

在存档中创建单个条目。

```csharp
public SevenZipArchiveEntry CreateEntry(string name, FileInfo fileInfo, 
    bool openImmediately = false, SevenZipEntrySettings newEntrySettings = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 条目的名称。 |
| fileInfo | FileInfo | 要压缩的文件的元数据。 |
| openImmediately | Boolean | 如果立即打开文件则为真，否则在存档保存时打开文件。 |
| newEntrySettings | SevenZipEntrySettings | 用于添加的[`SevenZipArchiveEntry`](../../sevenziparchiveentry)项目的压缩和加密设置。 |

### 返回值

七个 Zip 条目实例。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| UnauthorizedAccessException | *fileInfo*是只读的或者是一个目录。 |
| DirectoryNotFoundException | 指定的路径无效，例如位于未映射的驱动器上。 |
| IOException | 文件已打开。 |

### 评论

条目名称仅在*name*参数中设置。*fileInfo*参数中提供的文件名不会影响条目名称。

如果使用*openImmediately*参数立即打开文件，它将被阻止，直到保存存档。

### 例子

用不同密码加密的条目组成存档。

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
        archive.CreateEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
        archive.CreateEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
        archive.Save(sevenZipFile);
    }
}
```

### 也可以看看

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* 命名空间 [Aspose.Zip.SevenZip](../../sevenziparchive)
* 部件 [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings, FileSystemInfo) {#createentry_2}

在存档中创建单个条目。

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings, FileSystemInfo fileInfo)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 条目的名称。 |
| source | Stream | 条目的输入流。 |
| newEntrySettings | SevenZipEntrySettings | 用于添加的[`SevenZipArchiveEntry`](../../sevenziparchiveentry)项目的压缩和加密设置。 |
| fileInfo | FileSystemInfo | 要压缩的文件或文件夹的元数据。 |

### 返回值

SevenZip 条目实例。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| InvalidOperationException | *source*和*fileInfo*均为 null 或*source*为空，*fileInfo*代表目录。 |

### 评论

条目名称仅在*name*参数中设置。*fileInfo*参数中提供的文件名不会影响条目名称。

*fileInfo*如果条目是目录，则可以参考DirectoryInfo。

### 例子

使用 LZMA2 压缩加密条目编写存档。

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF}), new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1")), new FileInfo("data1.bin")); 
        archive.Save(sevenZipFile);
    }
}
```

### 也可以看看

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* 命名空间 [Aspose.Zip.SevenZip](../../sevenziparchive)
* 部件 [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings) {#createentry_1}

在存档中创建单个条目。

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 条目的名称。 |
| source | Stream | 条目的输入流。 |
| newEntrySettings | SevenZipEntrySettings | 用于添加的[`SevenZipArchiveEntry`](../../sevenziparchiveentry)项目的压缩和加密设置。 |

### 返回值

Zip 条目实例。

### 例子

使用 LZMA2 压缩和加密所有条目来编写 7z 存档。

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.7z");
}
```

### 也可以看看

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* 命名空间 [Aspose.Zip.SevenZip](../../sevenziparchive)
* 部件 [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, SevenZipEntrySettings) {#createentry_3}

在存档中创建单个条目。

```csharp
public SevenZipArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    SevenZipEntrySettings newEntrySettings = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 条目的名称。 |
| path | String | 新文件的完全限定名，或要压缩的相对文件名。 |
| openImmediately | Boolean | 如果立即打开文件则为真，否则在存档保存时打开文件。 |
| newEntrySettings | SevenZipEntrySettings | 用于添加的[`SevenZipArchiveEntry`](../../sevenziparchiveentry)项目的压缩和加密设置。 |

### 返回值

Zip 条目实例。

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

条目名称仅在*name*参数中设置。*path*参数中提供的文件名不影响条目名称。

如果使用*openImmediately*参数立即打开文件，它将被阻止，直到保存存档。

### 例子

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings())))
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### 也可以看看

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* 命名空间 [Aspose.Zip.SevenZip](../../sevenziparchive)
* 部件 [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
