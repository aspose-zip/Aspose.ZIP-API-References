---
title: "LzxArchiveEntry"
second_title: "Aspose.ZIP for Java API Referansı"
description: "LZX arşivi içinde tek bir dosyayı temsil eder."
type: docs
weight: 90
url: /tr/java/com.aspose.zip/lzxarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LzxArchiveEntry implements IArchiveFileEntry
```

LZX arşivi içinde tek bir dosyayı temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Girdiyi sağlanan akıma çıkarır. |
| [extract(String path)](#extract-java.lang.String-) | Lzx arşiv girdisini yola göre bir dosya sistemine çıkarır. |
| [getCommentary()](#getCommentary--) | Yorumu alır. |
| [getCompressedSize()](#getCompressedSize--) | Sıkıştırılmış dosyanın boyutunu alır. |
| [getLength()](#getLength--) | Girdinin uzunluğunu bayt cinsinden alır. |
| [getModificationTime()](#getModificationTime--) | Girişin son değiştirilme zamanını alır. |
| [getName()](#getName--) | Girişin adını alır. |
| [getUncompressedSize()](#getUncompressedSize--) | Orijinal dosyanın boyutunu alır. |
| [isDirectory()](#isDirectory--) | Bu girişin bir dizin olup olmadığını gösteren bir değer alır. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Girdiyi sağlanan akıma çıkarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hedef | java.io.OutputStream | Hedef akış. Yazılabilir olmalıdır. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Lzx arşiv girdisini yola göre bir dosya sistemine çıkarır.

```

``````

try (FileInputStream lzxFile = new FileInputStream("archive.lzx")) {
try (LzxArchive archive = new LzxArchive(lzxFile)) {
archive.getEntries().get(0).extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file which will store decompressed data. |

**Returns:**
java.io.File - FileSystemInfoInstance containing extracted data.
### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Gets size of the compressed file.

**Returns:**
long - size of the compressed file.
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
java.util.Date - the last modified time of the entry.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry.

Archives for compression only, such as gzip, bzip2, lzip, lzma, xz, z has name "File.bin" unless another name can be found in headers.

**Returns:**
java.lang.String - the name of the entry
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether this entry is a directory.

**Returns:**
boolean - a value indicating whether this entry is a directory.
