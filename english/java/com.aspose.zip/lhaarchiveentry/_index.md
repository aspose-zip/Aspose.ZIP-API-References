---
title: LhaArchiveEntry
second_title: Aspose.ZIP for Java API Reference
description: Represents single file within Lha archive.
type: docs
weight: 48
url: /java/com.aspose.zip/lhaarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LhaArchiveEntry implements IArchiveFileEntry
```

Represents single file within Lha archive.
## Methods

| Method | Description |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Extracts Lha archive entry to a file. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extracts the entry to the stream provided. |
| [extract(String path)](#extract-java.lang.String-) | Extracts Lha archive entry to a file by path. |
| [getLength()](#getLength--) | Gets the length of the entry in bytes. |
| [getName()](#getName--) | Gets the name of the entry. |
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
| file | java.io.File | File for storing decompressed data |

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


Extracts Lha archive entry to a file by path.

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
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry.

Archives for compression only, such as gzip, bzip2, lzip, lzma, xz, z has name "File.bin" unless another name can be found in headers.

**Returns:**
java.lang.String - the name of the entry
