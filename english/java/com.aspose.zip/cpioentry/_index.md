---
title: CpioEntry
second_title: Aspose.ZIP for Java API Reference
description: Represents single file within cpio archive.
type: docs
weight: 33
url: /java/com.aspose.zip/cpioentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CpioEntry implements IArchiveFileEntry
```

Represents single file within cpio archive.
## Methods

| Method | Description |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extracts the entry to the stream provided. |
| [extract(String path)](#extract-java.lang.String-) | Extracts the entry to the filesystem by the path provided. |
| [getLastWriteTimeUtc()](#getLastWriteTimeUtc--) | Gets the last write time. |
| [getLength()](#getLength--) | Gets the length of the entry in bytes. |
| [getName()](#getName--) | Gets the name of the entry within the archive. |
| [getParent()](#getParent--) | Gets the archive the entry belongs to. |
| [isDirectory()](#isDirectory--) | Gets a value indicating whether the entry represents a directory. |
| [open()](#open--) | Opens the entry for extraction and provides a stream with entry content. |
| [toString()](#toString--) | Returns string representation of the instance of the [CpioEntry](../../com.aspose.zip/cpioentry) class. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

Extract an entry of cpio archive.

```

     try (CpioArchive archive = new CpioArchive("archive.cpio")) {
         archive.getEntries().get(0).extract(httpResponseStream);
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

     try (CpioArchive archive = new CpioArchive("archive.cpio")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - the file info of the extracted file
### getLastWriteTimeUtc() {#getLastWriteTimeUtc--}
```
public final Date getLastWriteTimeUtc()
```


Gets the last write time.

**Returns:**
java.util.Date - the last write time
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


Gets the name of the entry within the archive.

**Returns:**
java.lang.String - the name of the entry within the archive
### getParent() {#getParent--}
```
public final CpioArchive getParent()
```


Gets the archive the entry belongs to.

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - the archive the entry belongs to
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory.
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with entry content.

Usage:

```

     CpioArchive archive = new CpioArchive("archive.cpio");
     CpioEntry entry = archive.getEntries().get(0);
     try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
         try (InputStream decompressed = entry.open()) {
             byte[] buffer = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
                 fileStream.write(buffer, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### toString() {#toString--}
```
public String toString()
```


Returns string representation of the instance of the [CpioEntry](../../com.aspose.zip/cpioentry) class.

**Returns:**
java.lang.String - string representation of this object.
