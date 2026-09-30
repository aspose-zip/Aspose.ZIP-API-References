---
title: "AppleArchiveEntry"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bir dosya veya dizin girdisini içinde temsil eder."
type: docs
weight: 17
url: /tr/java/com.aspose.zip/applearchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class AppleArchiveEntry implements IArchiveFileEntry
```

Bir dosya veya dizin girdisini bir [AppleArchive](../../com.aspose.zip/applearchive) içinde temsil eder.

Bu sınıfın bir örneği, mevcut bir Apple Arşivinden ayrıştırılan bir girdi ya da oluşturulan bir arşive eklenen bir girdi temsil edebilir.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Girdiyi sağlanan akıma çıkarır. |
| [extract(String path)](#extract-java.lang.String-) | Apple arşiv girdisini yola göre bir dosya sistemine çıkarır. |
| [getLength()](#getLength--) | Girdinin sıkıştırılmamış uzunluğunu bayt cinsinden alır. |
| [getName()](#getName--) | Girdinin arşiv içindeki yolunu alır. |
| [isDirectory()](#isDirectory--) | Girdinin bir dizin olup olmadığını gösteren değeri alır. |
| [open()](#open--) | Girdiyi çıkarma için açar ve girdinin içeriğini içeren bir akış sağlar. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


Girdiyi sağlanan akıma çıkarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hedef | java.io.OutputStream | hedef akış. Yazılabilir olmalıdır |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Apple arşiv girdisini yola göre bir dosya sistemine çıkarır.

```

``````

try (FileInputStream aaFile = new FileInputStream("archive.aa")) {
try (AppleArchive archive = new AppleArchive(aaFile)) {
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
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the uncompressed length of the entry in bytes.

For directory entries the value is zero. For entries created from a non-seekable source stream the length can be unknown.

**Returns:**
java.lang.Long - the uncompressed length of the entry in bytes.
### getName() {#getName--}
```
public final String getName()
```


Gets the path of the entry inside the archive.

The value is the archive path recorded for the entry. Directory entries usually end with Forward slash (`/`).

**Returns:**
java.lang.String - the path of the entry inside the archive.
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


Opens the entry for extraction and provides a stream with the entry content.

**Returns:**
java.io.InputStream - A readable stream that contains the extracted entry data.
