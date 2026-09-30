---
title: "AppleArchive"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bu sınıf bir Apple Archive .aar dosyasını temsil eder."
type: docs
weight: 16
url: /tr/java/com.aspose.zip/applearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AppleArchive implements IArchive, AutoCloseable
```

Bu sınıf bir Apple Archive (.aar) dosyasını temsil eder. Apple Archive dosyaları oluşturmak için kullanın.

Apple ve Apple Archive, Apple Inc.'in ticari markalarıdır.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [AppleArchive()](#AppleArchive--) | Oluşturulan girişler için kullanılan ayarlarla [AppleArchive](../../com.aspose.zip/applearchive) sınıfının yeni bir örneğini başlatır. |
| [AppleArchive(AppleArchiveEntrySettings newEntrySettings)](#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-) | Oluşturulan girişler için kullanılan ayarlarla [AppleArchive](../../com.aspose.zip/applearchive) sınıfının yeni bir örneğini başlatır. |
| [AppleArchive(InputStream sourceStream)](#AppleArchive-java.io.InputStream-) | Arşivden çıkarılabilecek bir giriş listesi oluşturur ve [AppleArchive](../../com.aspose.zip/applearchive) sınıfının yeni bir örneğini başlatır. |
| [AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-) | Arşivden çıkarılabilecek bir giriş listesi oluşturur ve [AppleArchive](../../com.aspose.zip/applearchive) sınıfının yeni bir örneğini başlatır. |
| [AppleArchive(String path)](#AppleArchive-java.lang.String-) | Arşivden çıkarılabilecek bir giriş listesi oluşturur ve [AppleArchive](../../com.aspose.zip/applearchive) sınıfının yeni bir örneğini başlatır. |
| [AppleArchive(String path, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-) | Arşivden çıkarılabilecek bir giriş listesi oluşturur ve [AppleArchive](../../com.aspose.zip/applearchive) sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler. |
| [createEntry(String name, File fileInfo)](#createEntry-java.lang.String-java.io.File-) | Arşiv içinde tek bir giriş oluşturur. |
| [createEntry(String name, File fileInfo, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Arşiv içinde tek bir giriş oluşturur. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Arşiv içinde tek bir giriş oluşturur. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Arşiv içinde tek bir giriş oluşturur. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Arşiv içinde tek bir giriş oluşturur. |
| [dispose()](#dispose--) | Yönetilmeyen kaynakların serbest bırakılması, bırakılması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Arşivdeki tüm dosyaları verilen dizine çıkarır. |
| [getEntries()](#getEntries--) | Arşivi oluşturan girişleri alır. |
| [getFileEntries()](#getFileEntries--) | Arşivi oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) türündeki girişleri alır. |
| [getFormat()](#getFormat--) | Arşiv biçimini alır. |
| [getNewEntrySettings()](#getNewEntrySettings--) | Yeni oluşturulan girişler için kullanılan ayarları alır. |
| [isSolid()](#isSolid--) | Arşivin katı sıkıştırma kullanıp kullanmadığını gösteren bir değeri alır. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Sağlanan akışa arşivi kaydeder. |
| [save(String destinationFileName)](#save-java.lang.String-) | Arşivi sağlanan hedef dosyaya kaydeder. |
### AppleArchive() {#AppleArchive--}
```
public AppleArchive()
```


Oluşturulan girişler için kullanılan ayarlarla [AppleArchive](../../com.aspose.zip/applearchive) sınıfının yeni bir örneğini başlatır.

### AppleArchive(AppleArchiveEntrySettings newEntrySettings) {#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-}
```
public AppleArchive(AppleArchiveEntrySettings newEntrySettings)
```


Oluşturulan girişler için kullanılan ayarlarla [AppleArchive](../../com.aspose.zip/applearchive) sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| newEntrySettings | [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) | Yeni bir Apple Archive oluşturulurken kullanılan ayarlar. |

### AppleArchive(InputStream sourceStream) {#AppleArchive-java.io.InputStream-}
```
public AppleArchive(InputStream sourceStream)
```


Arşivden çıkarılabilecek bir giriş listesi oluşturur ve [AppleArchive](../../com.aspose.zip/applearchive) sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | sourceStream | java.io.InputStream | Arşivin kaynağı. |

Bu yapıcı hiçbir girişi açmaz. Açma işlemi için [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) ve [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) yöntemlerine bakın. |

### AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)
```


Arşivden çıkarılabilecek bir giriş listesi oluşturur ve [AppleArchive](../../com.aspose.zip/applearchive) sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Arşivin kaynağı. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Mevcut arşivi yüklemek için seçenekler. |

Bu yapıcı hiçbir girişi açmaz. Açma işlemi için [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) ve [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) yöntemlerine bakın. |

### AppleArchive(String path) {#AppleArchive-java.lang.String-}
```
public AppleArchive(String path)
```


Arşivden çıkarılabilecek bir giriş listesi oluşturur ve [AppleArchive](../../com.aspose.zip/applearchive) sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | path | java.lang.String | Arşiv dosyasına tam nitelikli veya göreli yol. |

Bu yapıcı hiçbir girişi açmaz. Açma işlemi için [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) ve [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) yöntemlerine bakın. |

### AppleArchive(String path, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(String path, AppleArchiveLoadOptions loadOptions)
```


Arşivden çıkarılabilecek bir giriş listesi oluşturur ve [AppleArchive](../../com.aspose.zip/applearchive) sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | Arşiv dosyasına tam nitelikli veya göreli yol. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Mevcut arşivi yüklemek için seçenekler. |

Bu yapıcı hiçbir girişi açmaz. Açma işlemi için [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) ve [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) yöntemlerine bakın. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final AppleArchive createEntries(File directory)
```


Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| directory | java.io.File | Sıkıştırılacak dizin. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final AppleArchive createEntries(File directory, boolean includeRootDirectory)
```


Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| directory | java.io.File | Sıkıştırılacak dizin. |
| includeRootDirectory | boolean | Kök dizinin kendisinin dahil edilip edilmeyeceğini gösterir. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntry(String name, File fileInfo) {#createEntry-java.lang.String-java.io.File-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo)
```


Arşiv içinde tek bir giriş oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Girişin adı. |
| fileInfo | java.io.File | Sıkıştırılacak dosyanın meta verileri. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, File fileInfo, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo, boolean openImmediately)
```


Arşiv içinde tek bir giriş oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Girişin adı. |
| fileInfo | java.io.File | Sıkıştırılacak dosyanın meta verileri. |
| openImmediately | boolean | Dosya hemen açılıyorsa True, aksi takdirde dosya arşiv kaydedilirken açılır. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final AppleArchiveEntry createEntry(String name, InputStream source)
```


Arşiv içinde tek bir giriş oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Girişin adı. |
| source | java.io.InputStream | Giriş için giriş akışı. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final AppleArchiveEntry createEntry(String name, String path)
```


Arşiv içinde tek bir giriş oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Girişin adı. |
| path | java.lang.String | Sıkıştırılacak dosyanın yolu. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final AppleArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Arşiv içinde tek bir giriş oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Girişin adı. |
| path | java.lang.String | Sıkıştırılacak dosyanın yolu. |
| openImmediately | boolean | Dosya hemen açılıyorsa True, aksi takdirde dosya arşiv kaydedilirken açılır. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### dispose() {#dispose--}
```
public final void dispose()
```


Yönetilmeyen kaynakların serbest bırakılması, bırakılması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Arşivdeki tüm dosyaları verilen dizine çıkarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Çıkarılan dosyaların yerleştirileceği dizinin yolu. |

### getEntries() {#getEntries--}
```
public final List<AppleArchiveEntry> getEntries()
```


Arşivi oluşturan girişleri alır.

**Returns:**
java.util.List&lt;com.aspose.zip.AppleArchiveEntry&gt; - arşivi oluşturan girişler.
### getFileEntries() {#getFileEntries--}
```
public Iterable<IArchiveFileEntry> getFileEntries()
```


Arşivi oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) türündeki girişleri alır.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - arşivi oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) tipindeki girişler
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Arşiv biçimini alır.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final AppleArchiveEntrySettings getNewEntrySettings()
```


Yeni oluşturulan girişler için kullanılan ayarları alır.

**Returns:**
[AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) - settings used for newly composed entries.
### isSolid() {#isSolid--}
```
public final boolean isSolid()
```


Arşivin katı sıkıştırma kullanıp kullanmadığını gösteren bir değer alır. Katı modda, tüm giriş verileri tek bir akış olarak sıkıştırılır ve bireysel giriş çıkarımı mümkün değildir. Bunun yerine [IArchive.ExtractToDirectory()](../../com.aspose.zip/iarchive\\#ExtractToDirectory--) kullanın.

**Returns:**
boolean - arşivin katı sıkıştırma kullanıp kullanmadığını gösteren bir değer.
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Sağlanan akışa arşivi kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | output | java.io.OutputStream | Hedef akış. |

`output` yazılabilir olmalıdır. LZ4 gibi bazı sıkıştırma ayarları ayrıca aranabilir bir akış gerektirir. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Arşivi sağlanan hedef dosyaya kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationFileName | java.lang.String | Oluşturulacak arşivin yolu. |

