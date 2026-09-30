---
title: "IArchive"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bu arayüz bir arşivi temsil eder."
type: docs
weight: 161
url: /tr/java/com.aspose.zip/iarchive/
---

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public interface IArchive extends AutoCloseable
```

Bu arayüz bir arşivi temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Arşivdeki tüm dosyaları verilen dizine çıkarır. |
| [getFileEntries()](#getFileEntries--) | Arşivi oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) türündeki girişleri alır. |
| [getFormat()](#getFormat--) | Arşiv biçimini alır. |
### close() {#close--}
```
public abstract void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public abstract void extractToDirectory(String destinationDirectory)
```


Arşivdeki tüm dosyaları verilen dizine çıkarır.

Dizin mevcut değilse, oluşturulacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Çıkarılan dosyaların yerleştirileceği dizinin yolu. |

### getFileEntries() {#getFileEntries--}
```
public abstract Iterable<IArchiveFileEntry> getFileEntries()
```


Arşivi oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) türündeki girişleri alır.

Sadece sıkıştırma için kullanılan arşivler, örneğin gzip, bzip2, lzip, lzma, lz4, xz, z, tek bir kayıt - arşivin kendisi - içerir.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - arşivi oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) türündeki girişler.
### getFormat() {#getFormat--}
```
public abstract ArchiveFormat getFormat()
```


Arşiv biçimini alır.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
