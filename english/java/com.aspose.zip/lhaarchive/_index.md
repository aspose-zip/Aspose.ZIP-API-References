---
title: LhaArchive
second_title: Aspose.ZIP for Java API Reference
description: This class represents LHA .lzh archive file.
type: docs
weight: 47
url: /java/com.aspose.zip/lhaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LhaArchive implements IArchive, AutoCloseable
```

This class represents LHA (.lzh) archive file.

Only following compression methods are supported:

    | ------ | --------------------------------------------- |
    | Method | Explanation                                   |
    | lh0    | Uncompressed                                  |
    | lh4    | 8 KiB sliding dictionary and static Huffman   |
    | lh5    | 16 KiB sliding dictionary and static Huffman  |
    | lh6    | 64 KiB sliding dictionary and static Huffman  |
    | lh7    | 128 KiB sliding dictionary and static Huffman |
    | lhx    | 1 Mib sliding dictionary and static Huffman   |
    | lhd    | Directory                                     |
## Constructors

| Constructor | Description |
| --- | --- |
| [LhaArchive(InputStream sourceStream)](#LhaArchive-java.io.InputStream-) | Initializes a new instance of the [LhaArchive](../../com.aspose.zip/lhaarchive) class and composes entries list can be extracted from the archive. |
| [LhaArchive(String path)](#LhaArchive-java.lang.String-) | Initializes a new instance of the [LhaArchive](../../com.aspose.zip/lhaarchive) class and composes entries list can be extracted from the archive. |
## Methods

| Method | Description |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extracts all the files and directories in the archive to the directory provided. |
| [getDirectories()](#getDirectories--) | Gets directory entries of [LhaDirectoryEntry](../../com.aspose.zip/lhadirectoryentry) type constituting the archive. |
| [getEntries()](#getEntries--) | Gets file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive. |
| [getFileEntries()](#getFileEntries--) | Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive. |
### LhaArchive(InputStream sourceStream) {#LhaArchive-java.io.InputStream-}
```
public LhaArchive(InputStream sourceStream)
```


Initializes a new instance of the [LhaArchive](../../com.aspose.zip/lhaarchive) class and composes entries list can be extracted from the archive.

This constructor does not decompress any entry. See [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### LhaArchive(String path) {#LhaArchive-java.lang.String-}
```
public LhaArchive(String path)
```


Initializes a new instance of the [LhaArchive](../../com.aspose.zip/lhaarchive) class and composes entries list can be extracted from the archive.

The following example extract an archive, then decompress first entry to a `MemoryStream`.

```

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LhaArchive archive = new LhaArchive("sample.lzh")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the fully qualified or the relative path to the archive file |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files and directories in the archive to the directory provided.

```

     try (LhaArchive archive = new LhaArchive("archive.lzh")) {
         archive.extractToDirectory("C:/extracted");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getDirectories() {#getDirectories--}
```
public final List<LhaDirectoryEntry> getDirectories()
```


Gets directory entries of [LhaDirectoryEntry](../../com.aspose.zip/lhadirectoryentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LhaDirectoryEntry&gt; - directory entries of [LhaDirectoryEntry](../../com.aspose.zip/lhadirectoryentry) type constituting the archive
### getEntries() {#getEntries--}
```
public final List<LhaArchiveEntry> getEntries()
```


Gets file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LhaArchiveEntry&gt; - file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.

Archives for compression only, such as gzip, bzip2, lzip, lzma, xz, z consist of the single record - the archive itself.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive
