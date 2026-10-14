---
title: "CabArchive.CreateEntry"
second_title: "Aspose.ZIP for .NET API 参考"
description: "CabArchive 方法。创建存档中的单个条目"
type: docs
weight: 40
url: /zh/net/aspose.zip.cab/cabarchive/createentry/
---
## CreateEntry(string, string, CabEntrySettings) {#createentry_3}

在存档中创建单个条目。

```csharp
public CabEntry CreateEntry(string name, string path, CabEntrySettings newEntrySettings = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 条目的名称。 |
| 路径 | String | 新文件的完全限定名称，或要压缩的相对文件名。 |
| newEntrySettings | CabEntrySettings | 用于添加的 [`CabEntry`](../../cabentry/) 项目的压缩和加密设置。 |

### Return Value

Cab 条目实例。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *path* 为 null。 |
| SecurityException | 调用方没有访问所需的权限。 |
| ArgumentException | 该 *path* 为空，仅包含空白字符，或包含无效字符。 |
| UnauthorizedAccessException | 对文件 *path* 的访问被拒绝。 |
| PathTooLongException | 指定的 *path*、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 位于 *path* 的文件在字符串中间包含冒号 (:)。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| InvalidOperationException | 存档已准备好进行提取，无法添加条目。 |

## 备注

*name* 参数唯一决定条目名称。*path* 参数提供的文件名不影响条目名称。

## 示例

```csharp
using (var archive = new CabArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.cab");
}
```

### 另请参阅

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, CabEntrySettings) {#createentry_2}

在存档中创建单个条目。

```csharp
public CabEntry CreateEntry(string name, Stream source, CabEntrySettings newEntrySettings = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 条目的名称。 |
| source | 流 | 条目的输入流。 |
| newEntrySettings | CabEntrySettings | 用于添加的 [`CabEntry`](../../cabentry/) 项目的压缩和加密设置。 |

### Return Value

Cab 条目实例。

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| InvalidOperationException | 存档已准备好进行提取，无法添加条目。 |
| ArgumentNullException | *name* 为 null。 |

## 示例

```csharp
using (var archive = new CabArchive())
{
    using (var dataStream = new MemoryStream(File.ReadAllBytes("data.bin")))
    {
        archive.CreateEntry("stream-entry.bin", dataStream);
        archive.Save("archive.cab");
    }
}
```

```csharp
using (var archive = new CabArchive())
{     
    var settings = new CabEntrySettings(new CabStoreCompressionSettings());
    archive.CreateEntry("stream-entry.bin", dataStream, settings);
    archive.Save("archive.cab");     
}
```

### 另请参阅

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, CabEntrySettings) {#createentry_1}

在存档中创建单个条目。

```csharp
public CabEntry CreateEntry(string name, FileInfo fileInfo, 
    CabEntrySettings newEntrySettings = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 条目的名称。 |
| fileInfo | FileInfo | 待压缩文件的元数据。 |
| newEntrySettings | CabEntrySettings | 用于添加的 [`CabEntry`](../../cabentry/) 项目的压缩和加密设置。 |

### Return Value

CAB 条目实例。

### 异常

| 异常 | 条件 |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* 为只读或是目录。 |
| DirectoryNotFoundException | 指定的路径无效，例如位于未映射的驱动器上。 |
| IOException | 该文件已打开。 |
| FileNotFoundException | *fileInfo* 表示一个找不到的文件。 |
| SecurityException | 调用方没有访问 *fileInfo* 所需的权限。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| InvalidOperationException | 存档已准备好进行提取，无法添加条目。 |
| ArgumentNullException | *name* 为 null。 |

## 备注

*name* 参数唯一决定条目名称。*fileInfo* 参数提供的文件名不影响条目名称。

## 示例

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{
    var sourceFile = new FileInfo("logs\\log.txt");
    archive.CreateEntry("log.txt", sourceFile);
    archive.Save("archive.cab");
}
```

### 另请参阅

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, CabEntrySettings) {#createentry}

在存档中创建单个条目。

```csharp
public CabEntry CreateEntry(string name, Func<Stream> streamProvider, 
    CabEntrySettings newEntrySettings = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 条目的名称。 |
| streamProvider | Func`1 | 为条目提供输入流的方法。 |
| newEntrySettings | CabEntrySettings | 用于添加的 [`CabEntry`](../../cabentry/) 项目的压缩和加密设置。 |

### Return Value

CAB 条目实例。

### 异常

| 异常 | 条件 |
| --- | --- |
| InvalidOperationException | 存档已实例化用于解压缩。- 或 - 文件数量已达到上限。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| ArgumentException | *name* 为 null 或为空。 |

## 示例

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{    
    archive.CreateEntry("data.bin", provider);
    archive.Save("archive.cab");
}
```

### 另请参阅

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


