---
title: "WimArchive"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bu sınıf bir wim arşiv dosyasını temsil eder."
type: docs
weight: 130
url: /tr/java/com.aspose.zip/wimarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class WimArchive implements IArchive, AutoCloseable
```

Bu sınıf bir wim arşiv dosyasını temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [WimArchive(InputStream sourceStream)](#WimArchive-java.io.InputStream-) | Yeni bir [WimArchive](../../com.aspose.zip/wimarchive) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)](#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-) | Yeni bir [WimArchive](../../com.aspose.zip/wimarchive) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [WimArchive(String path)](#WimArchive-java.lang.String-) | Yeni bir [WimArchive](../../com.aspose.zip/wimarchive) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [WimArchive(String path, WimLoadOptions loadOptions)](#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-) | Yeni bir [WimArchive](../../com.aspose.zip/wimarchive) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Arşivi belirtilen yola dosya olarak çıkarır. |
| [getBootImageIndex()](#getBootImageIndex--) | Bootable (önyüklenebilir) görüntünün (sıfır tabanlı) indeksini alır. |
| [getEntries()](#getEntries--) | Arşivi oluşturan [WimEntry](../../com.aspose.zip/wimentry) türündeki girişleri alır. |
| [getFileEntries()](#getFileEntries--) | Wim arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) türündeki girişleri alır. |
| [getFileFormatVersion()](#getFileFormatVersion--) | Dosya formatının sürümünü alır. |
| [getFormat()](#getFormat--) | Arşiv biçimini alır. |
| [getGuid()](#getGuid--) | Arşiv için tanımlayıcı UUID'yi alır. |
| [getImages()](#getImages--) | Arşivi oluşturan [WimImage](../../com.aspose.zip/wimimage) türündeki girişleri alır. |
| [getManifest()](#getManifest--) | Dosyayı ve içindeki görüntüleri tanımlayan gömülü manifestoyu alır. |
### WimArchive(InputStream sourceStream) {#WimArchive-java.io.InputStream-}
```
public WimArchive(InputStream sourceStream)
```


Yeni bir [WimArchive](../../com.aspose.zip/wimarchive) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

Aşağıdaki örnek, tüm girişlerin bir dizine nasıl çıkarılacağını gösterir.

```

``````

try (WimArchive archive = new WimArchive(new FileInputStream("archive.wim"))) {
archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### WimArchive(InputStream sourceStream, WimLoadOptions loadOptions) {#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive(new FileInputStream("archive.wim"))) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Bu yapıcı hiçbir girişi açmaz. Açma işlemi için [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceStream | java.io.InputStream | arşivin kaynağı |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | Mevcut arşivi yüklemek için seçenekler. |

### WimArchive(String path) {#WimArchive-java.lang.String-}
```
public WimArchive(String path)
```


Yeni bir [WimArchive](../../com.aspose.zip/wimarchive) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

Aşağıdaki örnek, tüm girişlerin bir dizine nasıl çıkarılacağını gösterir.

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### WimArchive(String path, WimLoadOptions loadOptions) {#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(String path, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive("archive.wim")) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     }
 
```

Bu yapıcı hiçbir girişi açmaz. Açma işlemi için [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | arşiv dosyasının yolu |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | Mevcut arşivi yüklemek için seçenekler. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Arşivi belirtilen yola dosya olarak çıkarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationDirectory | java.lang.String | çıkarılan dosyaların yerleştirileceği dizinin yolu |

### getBootImageIndex() {#getBootImageIndex--}
```
public final int getBootImageIndex()
```


Bootable (önyüklenebilir) görüntünün (sıfır tabanlı) indeksini alır.

**Returns:**
int - önyüklenebilir görüntünün (sıfır tabanlı) dizini
### getEntries() {#getEntries--}
```
public final List<WimEntry> getEntries()
```


Arşivi oluşturan [WimEntry](../../com.aspose.zip/wimentry) türündeki girişleri alır.

**Returns:**
java.util.List&lt;com.aspose.zip.WimEntry&gt; - arşivi oluşturan girişler
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Wim arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) türündeki girişleri alır.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - wim arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) türündeki girişler
### getFileFormatVersion() {#getFileFormatVersion--}
```
public final int getFileFormatVersion()
```


Dosya formatının sürümünü alır.

**Returns:**
int - dosya formatının sürümü
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Arşiv biçimini alır.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Arşiv için tanımlayıcı UUID'yi alır.

**Returns:**
java.util.UUID - arşiv için tanımlayıcı UUID
### getImages() {#getImages--}
```
public final List<WimImage> getImages()
```


Arşivi oluşturan [WimImage](../../com.aspose.zip/wimimage) türündeki girişleri alır.

**Returns:**
java.util.List&lt;com.aspose.zip.WimImage&gt; - arşivi oluşturan [WimImage](../../com.aspose.zip/wimimage) türündeki girişler
### getManifest() {#getManifest--}
```
public final String getManifest()
```


Dosyayı ve içindeki görüntüleri tanımlayan gömülü manifestoyu alır.

**Returns:**
java.lang.String - dosyayı ve içerilen görüntüleri tanımlayan gömülü manifest
