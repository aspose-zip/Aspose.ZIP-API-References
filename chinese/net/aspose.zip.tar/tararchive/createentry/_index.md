---
title: TarArchive.CreateEntry
second_title: Aspose.ZIP for .NET API 参考
description: TarArchive 方法. 在存档中创建单个条目
type: docs
weight: 80
url: /zh/net/aspose.zip.tar/tararchive/createentry/
---
## CreateEntry(string, Stream, FileSystemInfo) {#createentry_1}

在存档中创建单个条目。

```csharp
public TarEntry CreateEntry(string name, Stream source, FileSystemInfo fileInfo = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 条目的名称。 |
| source | Stream | 条目的输入流。 |
| fileInfo | FileSystemInfo | 要压缩的文件或文件夹的元数据。 |

### 返回值

Tar 条目实例。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| PathTooLongException | *name*对于 IEEE 1003.1-1998 标准的 tar 来说太长了。 |
| ArgumentException | 文件名，作为的一部分*name*超过 100 个符号。 |

### 评论

条目名称仅在*name*范围。中提供的文件名*fileInfo*参数不影响条目名称。

*fileInfo*可以参考DirectoryInfo如果条目是目录。

### 例子

```csharp
using (var archive = new TarArchive())
{
   archive.CreateEntry("bytes", new MemoryStream(new byte[] {0x00, 0xFF}));
   archive.Save(tarFile);
}
```

### 也可以看看

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* 命名空间 [Aspose.Zip.Tar](../../tararchive/)
* 部件 [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

在存档中创建单个条目。

```csharp
public TarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 条目的名称。 |
| fileInfo | FileInfo | 要压缩的文件或文件夹的元数据。 |
| openImmediately | Boolean | 如果立即打开文件则为真，否则在存档保存时打开文件。 |

### 返回值

Tar 条目实例。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| PathTooLongException | *name*对于 IEEE 1003.1-1998 标准的 tar 来说太长了。 |
| ArgumentException | 文件名，作为的一部分*name*超过 100 个符号。 |

### 评论

条目名称仅在*name*范围。中提供的文件名*fileInfo*参数不影响条目名称。

*fileInfo*可以参考DirectoryInfo如果条目是目录。

如果文件立即打开*openImmediately*参数它会被阻塞，直到归档被处理。

### 例子

```csharp
FileInfo fi = new FileInfo("data.bin");
using (var archive = new TarArchive())
{
   archive.CreateEntry("data.bin", fi);
   archive.Save(tarFile);
}
```

### 也可以看看

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* 命名空间 [Aspose.Zip.Tar](../../tararchive/)
* 部件 [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

在存档中创建单个条目。

```csharp
public TarEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 条目的名称。 |
| path | String | 要压缩的文件的路径。 |
| openImmediately | Boolean | 如果立即打开文件则为真，否则在存档保存时打开文件。 |

### 返回值

Tar 条目实例。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *path*一片空白。 |
| SecurityException | 调用者没有所需的访问权限。 |
| ArgumentException | 这*path*为空、仅包含空格或包含无效字符。 - 或 - 文件名，作为*name*超过 100 个符号。 |
| UnauthorizedAccessException | 访问文件*path*被拒绝。 |
| PathTooLongException | 指定的*path*、文件名或两者都超过了系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 - 或者 -*name*对于 IEEE 1003.1-1998 标准的 tar 来说太长了。 |
| NotSupportedException | 归档于*path*在字符串中间包含一个冒号 (:)。 |

### 评论

条目名称仅在*name*范围。中提供的文件名*path*参数不影响条目名称。

如果文件立即打开*openImmediately*参数它会被阻塞，直到归档被处理。

### 例子

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save(outputTarFile);
}
```

### 也可以看看

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* 命名空间 [Aspose.Zip.Tar](../../tararchive/)
* 部件 [Aspose.Zip](../../../)


