---
title: Archive.CreateEntry
second_title: Aspose.ZIP for .NET API 参考
description: Archive 方法. 在存档中创建单个条目
type: docs
weight: 50
url: /zh/net/aspose.zip/archive/createentry/
---
## CreateEntry(string, string, bool, ArchiveEntrySettings) {#createentry_3}

在存档中创建单个条目。

```csharp
public ArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 条目的名称。 |
| path | String | 新文件的完全限定名称，或要压缩的相对文件名。 |
| openImmediately | Boolean | 如果立即打开文件则为真，否则在存档保存时打开文件。 |
| newEntrySettings | ArchiveEntrySettings | 用于添加的压缩和加密设置[`ArchiveEntry`](../../archiveentry/)物品。 |

### 返回值

Zip 条目实例。

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

条目名称仅在*name*范围。中提供的文件名*path*参数不影响条目名称。

如果文件立即打开*openImmediately*参数它会被阻止，直到存档被保存。

### 例子

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

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* 命名空间 [Aspose.Zip](../../archive/)
* 部件 [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings) {#createentry_1}

在存档中创建单个条目。

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, 
    ArchiveEntrySettings newEntrySettings = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 条目的名称。 |
| source | Stream | 条目的输入流。 |
| newEntrySettings | ArchiveEntrySettings | 用于添加的压缩和加密设置[`ArchiveEntry`](../../archiveentry/)物品。 |

### 返回值

Zip 条目实例。

### 例子

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.zip");
}
```

### 也可以看看

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* 命名空间 [Aspose.Zip](../../archive/)
* 部件 [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool, ArchiveEntrySettings) {#createentry}

在存档中创建单个条目。

```csharp
public ArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 条目的名称。 |
| fileInfo | FileInfo | 要压缩的文件的元数据。 |
| openImmediately | Boolean | 如果立即打开文件则为真，否则在存档保存时打开文件。 |
| newEntrySettings | ArchiveEntrySettings | 用于添加的压缩和加密设置[`ArchiveEntry`](../../archiveentry/)物品。 |

### 返回值

Zip 条目实例。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| UnauthorizedAccessException | *fileInfo*是只读的或者是一个目录。 |
| DirectoryNotFoundException | 指定的路径无效，例如在未映射的驱动器上。 |
| IOException | 该文件已经打开。 |

### 评论

条目名称仅在*name*范围。中提供的文件名*fileInfo*参数不影响条目名称。

如果文件立即打开*openImmediately*参数它会被阻止，直到存档被保存。

### 例子

用不同的加密方法和密码加密的条目组成存档。

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
        archive.CreateEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass2", EncryptionMethod.AES128)));
        archive.CreateEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass3", EncryptionMethod.AES256)));
        archive.Save(zipFile);
    }
}
```

### 也可以看看

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* 命名空间 [Aspose.Zip](../../archive/)
* 部件 [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings, FileSystemInfo) {#createentry_2}

在存档中创建单个条目。

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, ArchiveEntrySettings newEntrySettings, 
    FileSystemInfo fileInfo)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 条目的名称。 |
| source | Stream | 条目的输入流。 |
| newEntrySettings | ArchiveEntrySettings | 用于添加的压缩和加密设置[`ArchiveEntry`](../../archiveentry/)物品。 |
| fileInfo | FileSystemInfo | 要压缩的文件或文件夹的元数据。 |

### 返回值

Zip 条目实例。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| InvalidOperationException | 两个都*source*和*fileInfo*为空或*source*为空且*fileInfo*代表目录。 |

### 评论

条目名称仅在*name*范围。中提供的文件名*fileInfo*参数不影响条目名称。

*fileInfo*可以参考DirectoryInfo如果条目是目录。

### 例子

使用加密条目撰写存档。

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF} ), new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")), new FileInfo("data1.bin")); 
        archive.Save(zipFile);
    }
}
```

### 也可以看看

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* 命名空间 [Aspose.Zip](../../archive/)
* 部件 [Aspose.Zip](../../../)


