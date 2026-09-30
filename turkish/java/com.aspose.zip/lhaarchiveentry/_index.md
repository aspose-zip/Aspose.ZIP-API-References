---
title: "LhaArchiveEntry"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Lha arşivi içinde tek bir dosyayı temsil eder."
type: docs
weight: 76
url: /tr/java/com.aspose.zip/lhaarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LhaArchiveEntry implements IArchiveFileEntry
```

Lha arşivi içinde tek bir dosyayı temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Lha arşiv girişini bir dosyaya çıkarır. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Girdiyi sağlanan akıma çıkarır. |
| [extract(String path)](#extract-java.lang.String-) | Lha arşiv girişini yol ile bir dosya sistemine çıkarır. |
| [getLastModified()](#getLastModified--) | Girişin son değiştirilme zamanını alır. |
| [getLength()](#getLength--) | Girdinin uzunluğunu bayt cinsinden alır. |
| [getModificationTime()](#getModificationTime--) | Girişin son değiştirilme zamanını alır. |
| [getName()](#getName--) | Girişin adını alır. |
| [getPath()](#getPath--) | Girişin tam yolunu alır. |
| [isDirectory()](#isDirectory--) | Bu girişin bir dizin olup olmadığını gösteren bir değer alır. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Lha arşiv girişini bir dosyaya çıkarır.

```

``````

try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
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

``````

     try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
         try (LhaArchive archive = new LhaArchive(lhaFile)) {
             archive.getEntries().get(0).extract("extracted.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | açılmış verileri depolayacak dosyanın yolu |

**Returns:**
java.io.File - çıkarılan veriyi içeren java.io.File örneği
### getLastModified() {#getLastModified--}
```
public final Date getLastModified()
```


Girişin son değiştirilme zamanını alır.

**Returns:**
java.util.Date - girdinin son değiştirilme zamanı
### getLength() {#getLength--}
```
public final Long getLength()
```


Girdinin uzunluğunu bayt cinsinden alır.

**Returns:**
java.lang.Long - girişin bayt cinsinden uzunluğu
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Girişin son değiştirilme zamanını alır.

**Returns:**
java.util.Date - girdinin son değiştirilme zamanı
### getName() {#getName--}
```
public final String getName()
```


Girişin adını alır.

Sıkıştırma amaçlı arşivler, örneğin gzip, bzip2, lzip, lzma, xz, z, başlıklarda başka bir ad bulunmadığı sürece "File.bin" adını alır.

**Returns:**
java.lang.String - girişin adı
### getPath() {#getPath--}
```
public final String getPath()
```


Girişin tam yolunu alır.

**Returns:**
java.lang.String - girdinin tam yolu
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Bu girişin bir dizin olup olmadığını gösteren bir değer alır.

**Returns:**
boolean - bu girdinin bir dizin olup olmadığını gösteren değer.
