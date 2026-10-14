---
title: "IArchive"
second_title: "Aspose.ZIP for Java API 参考"
description: "此接口表示一个存档。"
type: docs
weight: 161
url: /zh/java/com.aspose.zip/iarchive/
---

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public interface IArchive extends AutoCloseable
```

此接口表示一个存档。
## 方法

| 方法 | 描述 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将存档中的所有文件提取到提供的目录。 |
| [getFileEntries()](#getFileEntries--) | 获取构成存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。 |
| [getFormat()](#getFormat--) | 获取存档格式。 |
### close() {#close--}
```
public abstract void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public abstract void extractToDirectory(String destinationDirectory)
```


将存档中的所有文件提取到提供的目录。

如果目录不存在，将会被创建。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationDirectory | java.lang.String | 用于放置解压文件的目录路径。 |

### getFileEntries() {#getFileEntries--}
```
public abstract Iterable<IArchiveFileEntry> getFileEntries()
```


获取构成存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。

仅用于压缩的归档，例如 gzip、bzip2、lzip、lzma、lz4、xz、z，仅包含单个记录——即归档本身。

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - 构成存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。
### getFormat() {#getFormat--}
```
public abstract ArchiveFormat getFormat()
```


获取存档格式。

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
