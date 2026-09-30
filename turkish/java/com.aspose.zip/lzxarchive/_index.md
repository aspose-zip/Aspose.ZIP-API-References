---
title: "LzxArchive"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bu sınıf bir LZX .lzx arşiv dosyasını temsil eder."
type: docs
weight: 89
url: /tr/java/com.aspose.zip/lzxarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LzxArchive implements IArchive, AutoCloseable
```

Bu sınıf bir LZX (.lzx) arşiv dosyasını temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [LzxArchive(InputStream extractionSource)](#LzxArchive-java.io.InputStream-) | Yeni bir [LzxArchive](../../com.aspose.zip/lzxarchive) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)](#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-) | Yeni bir [LzxArchive](../../com.aspose.zip/lzxarchive) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [LzxArchive(String path)](#LzxArchive-java.lang.String-) | Yeni bir [LzxArchive](../../com.aspose.zip/lzxarchive) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [LzxArchive(String path, LzxLoadOptions loadOptions)](#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-) | Yeni bir [LzxArchive](../../com.aspose.zip/lzxarchive) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Arşivdeki tüm dosya ve dizinleri verilen dizine çıkarır. |
| [getEntries()](#getEntries--) | [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) tipindeki dosya girişlerini alır ve arşivi oluşturur. |
| [getFileEntries()](#getFileEntries--) | Arşivi oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) türündeki girişleri alır. |
| [getFormat()](#getFormat--) | Arşiv biçimini alır. |
### LzxArchive(InputStream extractionSource) {#LzxArchive-java.io.InputStream-}
```
public LzxArchive(InputStream extractionSource)
```


Yeni bir [LzxArchive](../../com.aspose.zip/lzxarchive) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

Bu yapıcı herhangi bir girişi açmaz. Açma işlemi için [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\\#extract-OutputStream-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| extractionSource | java.io.InputStream | Arşivin kaynağı. |

### LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions) {#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)
```


Yeni bir [LzxArchive](../../com.aspose.zip/lzxarchive) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

Bu yapıcı herhangi bir girişi açmaz. Açma işlemi için [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\\#extract-OutputStream-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| extractionSource | java.io.InputStream | Arşivin kaynağı. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | Mevcut arşivi yüklemek için seçenekler. |

### LzxArchive(String path) {#LzxArchive-java.lang.String-}
```
public LzxArchive(String path)
```


Yeni bir [LzxArchive](../../com.aspose.zip/lzxarchive) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

Aşağıdaki örnek bir arşivi çıkarır, ardından ilk girişi bir `MemoryStream`'e açar.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LzxArchive archive = new LzxArchive("sample.lzx")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |

### LzxArchive(String path, LzxLoadOptions loadOptions) {#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(String path, LzxLoadOptions loadOptions)
```


Initializes a new instance of the [LzxArchive](../../com.aspose.zip/lzxarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LzxArchive archive = new LzxArchive("sample.lzx")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

Bu yapıcı herhangi bir girişi açmaz. Açma işlemi için [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\\#extract-OutputStream-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | Arşiv dosyasına tam nitelikli veya göreli yol. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | Mevcut arşivi yüklemek için seçenekler. |

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

try (LzxArchive archive = new LzxArchive("archive.lzx")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getEntries() {#getEntries--}
```
public final List<LzxArchiveEntry> getEntries()
```


Gets file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LzxArchiveEntry&gt; - file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.
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
