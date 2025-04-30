---
title: LhaArchiveEntry
second_title: Aspose.ZIP for Java API Reference
description: Represents a single file within Lha archive.
type: docs
weight: 50
url: /java/com.aspose.zip/lhaarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LhaArchiveEntry implements IArchiveFileEntry
```

Represents a single file within Lha archive.
## Methods

| Method | Description |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Extracts Lha archive entry to a file. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extracts the entry to the stream provided. |
| [extract(String path)](#extract-java.lang.String-) | Extracts Lha archive entry to a filesystem by path. |
| [getLastModified()](#getLastModified--) | Gets the last modified time of the entry. |
| [getLength()](#getLength--) | Gets the length of the entry in bytes. |
| [getModificationTime()](#getModificationTime--) | Gets the last modified time of the entry. |
| [getName()](#getName--) | Gets the name of the entry. |
| [getPath()](#getPath--) | Gets the full path to the entry. |
| [isDirectory()](#isDirectory--) | Gets a value indicating whether this entry directory. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extracts Lha archive entry to a file.

```

     try (FileInputStream lhaFile = new FileInputStream("archive.lzh")) {
         try (LhaArchive archive = new LhaArchive(lhaFile)) {
             archive.getEntries().get(0).extract(new File("extracted.bin"));
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | File for storing decompressed data.

Does nothing for directory entry |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts Lha archive entry to a filesystem by path.

```

     try (FileInputStream lhaFile = new FileInputStream("archive.lzh")) {
         try (LhaArchive archive = new LhaArchive(lhaFile)) {
             archive.getEntries().get(0).extract("extracted.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file which will store decompressed data |

**Returns:**
java.io.File - java.io.File instance containing extracted data
### getLastModified() {#getLastModified--}
```
public final Date getLastModified()
```


Gets the last modified time of the entry.

**Returns:**
java.util.Date - the last modified time of the entry
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets the last modified time of the entry.

**Returns:**
java.util.Date - the last modified time of the entry
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry.

Archives for compression only, such as gzip, bzip2, lzip, lzma, xz, z has name "File.bin" unless another name can be found in headers.

**Returns:**
java.lang.String - the name of the entry
### getPath() {#getPath--}
```
public final String getPath()
```


Gets the full path to the entry.

**Returns:**
java.lang.String - the full path to the entry
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether this entry directory.

**Returns:**
boolean - a value indicating whether this entry directory.
