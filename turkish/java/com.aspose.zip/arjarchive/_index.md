---
title: "ArjArchive"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bu sınıf bir ARJ arşiv dosyasını temsil eder."
type: docs
weight: 37
url: /tr/java/com.aspose.zip/arjarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ArjArchive implements IArchive, AutoCloseable
```

Bu sınıf bir ARJ arşiv dosyasını temsil eder.

Yalnızca aşağıdaki sıkıştırma yöntemleri desteklenir:

| ------ | ------------------------------------------------------------ |
| Yöntem | Açıklama                                                  |
| 0      | Sıkıştırılmamış                                                 |
| 1      | LZ77 ve uyarlamalı Huffman kodlamasının kombinasyonu. En iyi oran. |
| 2      | LZ77 ve uyarlamalı Huffman kodlamasının kombinasyonu.             |
| 3      | LZ77 ve uyarlamalı Huffman kodlamasının kombinasyonu. En hızlı. |
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ArjArchive(InputStream extractionSource)](#ArjArchive-java.io.InputStream-) | Arşivden çıkarılabilecek bir giriş listesi oluşturan [ArjArchive](../../com.aspose.zip/arjarchive) sınıfının yeni bir örneğini başlatır. |
| [ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)](#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-) | Arşivden çıkarılabilecek bir giriş listesi oluşturan [ArjArchive](../../com.aspose.zip/arjarchive) sınıfının yeni bir örneğini başlatır. |
| [ArjArchive(String path)](#ArjArchive-java.lang.String-) | Arşivden çıkarılabilecek bir giriş listesi oluşturan [ArjArchive](../../com.aspose.zip/arjarchive) sınıfının yeni bir örneğini başlatır. |
| [ArjArchive(String path, ArjLoadOptions loadOptions)](#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-) | Arşivden çıkarılabilecek bir giriş listesi oluşturan [ArjArchive](../../com.aspose.zip/arjarchive) sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Tüm girişleri belirtilen dizine çıkarır. |
| [getCommentary()](#getCommentary--) | Yorumu alır. |
| [getEntries()](#getEntries--) | [ArjEntryPlain](../../com.aspose.zip/arjentryplain) türündeki girişleri alır ve ARJ arşivini oluşturur. |
| [getFileEntries()](#getFileEntries--) | Arşivi oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) türündeki girişleri alır. |
| [getFormat()](#getFormat--) | Arşiv biçimini alır. |
| [getName()](#getName--) | Orijinal adı alır. |
### ArjArchive(InputStream extractionSource) {#ArjArchive-java.io.InputStream-}
```
public ArjArchive(InputStream extractionSource)
```


Arşivden çıkarılabilecek bir giriş listesi oluşturan [ArjArchive](../../com.aspose.zip/arjarchive) sınıfının yeni bir örneğini başlatır.

Bu yapıcı hiçbir girişi açmaz. Açmak için [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| extractionSource | java.io.InputStream | arşivin kaynağı |

### ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions) {#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)
```


Arşivden çıkarılabilecek bir giriş listesi oluşturan [ArjArchive](../../com.aspose.zip/arjarchive) sınıfının yeni bir örneğini başlatır.

Bu yapıcı hiçbir girişi açmaz. Açmak için [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| extractionSource | java.io.InputStream | arşivin kaynağı |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | Mevcut arşivi yüklemek için seçenekler. |

### ArjArchive(String path) {#ArjArchive-java.lang.String-}
```
public ArjArchive(String path)
```


Arşivden çıkarılabilecek bir giriş listesi oluşturan [ArjArchive](../../com.aspose.zip/arjarchive) sınıfının yeni bir örneğini başlatır.

Aşağıdaki örnek, tüm girdileri bir dizine nasıl çıkarılacağını gösterir.

```

``````

try (ArjArchive archive = new ArjArchive("archive.arj")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### ArjArchive(String path, ArjLoadOptions loadOptions) {#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(String path, ArjLoadOptions loadOptions)
```


Initializes a new instance of the [ArjArchive](../../com.aspose.zip/arjarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (ArjArchive archive = new ArjArchive("archive.arj")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Bu yapıcı hiçbir girişi açmaz. Açmak için [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | arşiv dosyasının yolu |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | Mevcut arşivi yüklemek için seçenekler. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Tüm girişleri belirtilen dizine çıkarır.

Aşağıdaki örnek, tüm girişlerin bir dizine nasıl çıkarılacağını gösterir:

```

``````

try (ArjArchive archive = new ArjArchive(new FileInputStream("archive.arj"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the directory to extract the entries to |

### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getEntries() {#getEntries--}
```
public final List<ArjEntryPlain> getEntries()
```


Gets entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.

**Returns:**
java.util.List&lt;com.aspose.zip.ArjEntryPlain&gt; - entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.
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
### getName() {#getName--}
```
public final String getName()
```


Gets the original name.

**Returns:**
java.lang.String - the original name.
