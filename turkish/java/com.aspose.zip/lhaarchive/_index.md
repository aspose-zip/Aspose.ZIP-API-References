---
title: "LhaArchive"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bu sınıf bir LHA .lzh arşiv dosyasını temsil eder."
type: docs
weight: 75
url: /tr/java/com.aspose.zip/lhaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LhaArchive implements IArchive, AutoCloseable
```

Bu sınıf bir LHA (.lzh) arşiv dosyasını temsil eder.

Yalnızca aşağıdaki sıkıştırma yöntemleri desteklenir:

| ------ | --------------------------------------------- |
| Yöntem | Açıklama                                   |
| lh0    | Sıkıştırılmamış                                  |
| lh4    | 8 KiB kaydırmalı sözlük ve statik Huffman   |
| lh5    | 16 KiB kaydırmalı sözlük ve statik Huffman  |
| lh6    | 64 KiB kaydırmalı sözlük ve statik Huffman  |
| lh7    | 128 KiB kaydırmalı sözlük ve statik Huffman |
| lhx    | 1 Mib kaydırmalı sözlük ve statik Huffman   |
| lhd    | Dizin                                     |
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [LhaArchive(InputStream sourceStream)](#LhaArchive-java.io.InputStream-) | Yeni bir [LhaArchive](../../com.aspose.zip/lhaarchive) sınıfının örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)](#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-) | Yeni bir [LhaArchive](../../com.aspose.zip/lhaarchive) sınıfının örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [LhaArchive(String path)](#LhaArchive-java.lang.String-) | Yeni bir [LhaArchive](../../com.aspose.zip/lhaarchive) sınıfının örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [LhaArchive(String path, LhaLoadOptions loadOptions)](#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-) | Yeni bir [LhaArchive](../../com.aspose.zip/lhaarchive) sınıfının örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Arşivdeki tüm dosya ve dizinleri verilen dizine çıkarır. |
| [getEntries()](#getEntries--) | Arşivi oluşturan [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) tipindeki dosya girişlerini alır. |
| [getFileEntries()](#getFileEntries--) | Arşivi oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) türündeki girişleri alır. |
| [getFormat()](#getFormat--) | Arşiv biçimini alır. |
### LhaArchive(InputStream sourceStream) {#LhaArchive-java.io.InputStream-}
```
public LhaArchive(InputStream sourceStream)
```


Yeni bir [LhaArchive](../../com.aspose.zip/lhaarchive) sınıfının örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

Bu yapıcı herhangi bir girişi açmaz. Açmak için [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceStream | java.io.InputStream | arşivin kaynağı |

### LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions) {#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)
```


Yeni bir [LhaArchive](../../com.aspose.zip/lhaarchive) sınıfının örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

Bu yapıcı herhangi bir girişi açmaz. Açmak için [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceStream | java.io.InputStream | arşivin kaynağı |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | Mevcut arşivi yüklemek için seçenekler. |

### LhaArchive(String path) {#LhaArchive-java.lang.String-}
```
public LhaArchive(String path)
```


Yeni bir [LhaArchive](../../com.aspose.zip/lhaarchive) sınıfının örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

Aşağıdaki örnek bir arşivi çıkarır, ardından ilk girişi bir `MemoryStream`'e açar.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LhaArchive archive = new LhaArchive("sample.lzh")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the fully qualified or the relative path to the archive file |

### LhaArchive(String path, LhaLoadOptions loadOptions) {#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(String path, LhaLoadOptions loadOptions)
```


Initializes a new instance of the [LhaArchive](../../com.aspose.zip/lhaarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LhaArchive archive = new LhaArchive("sample.lzh")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

Bu yapıcı herhangi bir girişi açmaz. Açmak için [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | arşiv dosyasının tam nitelikli veya göreli yolu |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | Mevcut arşivi yüklemek için seçenekler. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Arşivdeki tüm dosya ve dizinleri verilen dizine çıkarır.

```

``````

try (LhaArchive archive = new LhaArchive("archive.lzh")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

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

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
