---
title: "AlzArchive"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bir ALZ arşiv dosyasını temsil eder."
type: docs
weight: 11
url: /tr/java/com.aspose.zip/alzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AlzArchive implements IArchive, AutoCloseable
```

Bir ALZ arşiv dosyasını temsil eder. Bu sınıfı ALZ arşivlerini incelemek ve çıkarmak için kullanın.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [AlzArchive(InputStream stream)](#AlzArchive-java.io.InputStream-) | Bir akıştan ALZ arşivi başlatır. |
| [AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-) | Sağlanan yükleme seçeneklerini kullanarak bir akıştan ALZ arşivi başlatır. |
| [AlzArchive(String filePath)](#AlzArchive-java.lang.String-) | Bir dosya yolundan ALZ arşivi başlatır. |
| [AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-) | Sağlanan yükleme seçeneklerini kullanarak bir dosya yolundan ALZ arşivi başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [close()](#close--) | Bu arşivin tuttuğu kaynakları serbest bırakır. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Tüm dosya ve dizinleri sağlanan dizine çıkarır. |
| [getEntries()](#getEntries--) | Bu arşivi oluşturan girdileri alır. |
| [getFileEntries()](#getFileEntries--) | Ortak arşiv arayüzü aracılığıyla girdileri alır. |
| [getFormat()](#getFormat--) | Arşiv biçimini alır. |
### AlzArchive(InputStream stream) {#AlzArchive-java.io.InputStream-}
```
public AlzArchive(InputStream stream)
```


Bir akıştan ALZ arşivi başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.InputStream | ALZ arşiv akışı; okuma ve arama desteklemelidir |

### AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)
```


Sağlanan yükleme seçeneklerini kullanarak bir akıştan ALZ arşivi başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.InputStream | ALZ arşiv akışı; okuma ve arama desteklemelidir |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | arşivi yüklemek için kullanılan seçenekler |

### AlzArchive(String filePath) {#AlzArchive-java.lang.String-}
```
public AlzArchive(String filePath)
```


Bir dosya yolundan ALZ arşivi başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | java.lang.String | ALZ arşivine giden yol |

### AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)
```


Sağlanan yükleme seçeneklerini kullanarak bir dosya yolundan ALZ arşivi başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | java.lang.String | ALZ arşivine giden yol |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | arşivi yüklemek için kullanılan seçenekler |

### close() {#close--}
```
public void close()
```


Bu arşivin tuttuğu kaynakları serbest bırakır.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Tüm dosya ve dizinleri sağlanan dizine çıkarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationDirectory | java.lang.String | hedef dizin; gerektiğinde oluşturulur |

### getEntries() {#getEntries--}
```
public final List<AlzEntry> getEntries()
```


Bu arşivi oluşturan girdileri alır.

**Returns:**
java.util.List&lt;com.aspose.zip.AlzEntry&gt; - ALZ girişlerinin değiştirilemez listesi
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Ortak arşiv arayüzü aracılığıyla girdileri alır.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - arşiv girişleri
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Arşiv biçimini alır.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - [ArchiveFormat.Alz](../../com.aspose.zip/archiveformat\#Alz)
