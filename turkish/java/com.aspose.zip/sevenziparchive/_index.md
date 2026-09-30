---
title: "SevenZipArchive"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bu sınıf 7z arşiv dosyasını temsil eder."
type: docs
weight: 104
url: /tr/java/com.aspose.zip/sevenziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class SevenZipArchive implements IArchive, AutoCloseable
```

Bu sınıf 7z arşiv dosyasını temsil eder. 7z arşivlerini oluşturmak ve çıkarmak için kullanın.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SevenZipArchive()](#SevenZipArchive--) | [SevenZipArchive](../../com.aspose.zip/sevenziparchive) sınıfının yeni bir örneğini girişleri için isteğe bağlı ayarlarla başlatır. |
| [SevenZipArchive(SevenZipEntrySettings newEntrySettings)](#SevenZipArchive-com.aspose.zip.SevenZipEntrySettings-) | [SevenZipArchive](../../com.aspose.zip/sevenziparchive) sınıfının yeni bir örneğini girişleri için isteğe bağlı ayarlarla başlatır. |
| [SevenZipArchive(InputStream sourceStream)](#SevenZipArchive-java.io.InputStream-) | Yeni bir [SevenZipArchive](../../com.aspose.zip/sevenziparchive) sınıfı örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [SevenZipArchive(InputStream sourceStream, String password)](#SevenZipArchive-java.io.InputStream-java.lang.String-) | Yeni bir [SevenZipArchive](../../com.aspose.zip/sevenziparchive) sınıfı örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [SevenZipArchive(String path)](#SevenZipArchive-java.lang.String-) | Yeni bir [SevenZipArchive](../../com.aspose.zip/sevenziparchive) sınıfı örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [SevenZipArchive(String path, String password)](#SevenZipArchive-java.lang.String-java.lang.String-) | Yeni bir [SevenZipArchive](../../com.aspose.zip/sevenziparchive) sınıfı örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [SevenZipArchive(InputStream sourceStream, SevenZipLoadOptions options)](#SevenZipArchive-java.io.InputStream-com.aspose.zip.SevenZipLoadOptions-) | Yeni bir [SevenZipArchive](../../com.aspose.zip/sevenziparchive) sınıfı örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [SevenZipArchive(String path, SevenZipLoadOptions options)](#SevenZipArchive-java.lang.String-com.aspose.zip.SevenZipLoadOptions-) | Yeni bir [SevenZipArchive](../../com.aspose.zip/sevenziparchive) sınıfı örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [SevenZipArchive(String[] parts)](#SevenZipArchive-java.lang.String---) | Çok bölümlü 7z arşivinden yeni bir [SevenZipArchive](../../com.aspose.zip/sevenziparchive) sınıfı örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [SevenZipArchive(String[] parts, String password)](#SevenZipArchive-java.lang.String---java.lang.String-) | Çok bölümlü 7z arşivinden yeni bir [SevenZipArchive](../../com.aspose.zip/sevenziparchive) sınıfı örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Arşiv içinde tek bir giriş oluşturur. |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Arşiv içinde tek bir giriş oluşturur. |
| [createEntry(String name, File file, boolean openImmediately, SevenZipEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.SevenZipEntrySettings-) | Arşiv içinde tek bir giriş oluşturur. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Arşiv içinde tek bir giriş oluşturur. |
| [createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.SevenZipEntrySettings-) | Arşiv içinde tek bir giriş oluşturur. |
| [createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings, File file)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.SevenZipEntrySettings-java.io.File-) | Arşiv içinde tek bir giriş oluşturur. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Arşiv içinde tek bir giriş oluşturur. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Arşiv içinde tek bir giriş oluşturur. |
| [createEntry(String name, String path, boolean openImmediately, SevenZipEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.SevenZipEntrySettings-) | Arşiv içinde tek bir giriş oluşturur. |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--) | Arşiv içinde tek bir giriş oluştur. |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, SevenZipEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.SevenZipEntrySettings-) | Arşiv içinde tek bir giriş oluştur. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Arşivdeki tüm dosyaları verilen dizine çıkarır. |
| [extractToDirectory(String destinationDirectory, String password)](#extractToDirectory-java.lang.String-java.lang.String-) | Arşivdeki tüm dosyaları verilen dizine çıkarır. |
| [getEntries()](#getEntries--) | Arşivi oluşturan [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) tipindeki girişleri alır. |
| [getFileEntries()](#getFileEntries--) | 7z arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) tipindeki girişleri alır. |
| [getFormat()](#getFormat--) | Arşiv biçimini alır. |
| [getNewEntrySettings()](#getNewEntrySettings--) | Yeni eklenen [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) öğeleri için kullanılan sıkıştırma ve şifreleme ayarları. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | 7z arşivini sağlanan akışa kaydeder. |
| [save(OutputStream output, SevenZipArchiveSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.SevenZipArchiveSaveOptions-) | 7z arşivini sağlanan akışa kaydeder. |
| [save(String destinationFileName)](#save-java.lang.String-) | Arşivi sağlanan hedef dosyaya kaydeder. |
| [save(String destinationFileName, SevenZipArchiveSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.SevenZipArchiveSaveOptions-) | Arşivi sağlanan hedef dosyaya kaydeder. |
| [saveSplit(String destinationDirectory, SplitSevenZipArchiveSaveOptions options)](#saveSplit-java.lang.String-com.aspose.zip.SplitSevenZipArchiveSaveOptions-) | Çok bölümlü arşivi sağlanan hedef dizine kaydeder. |
### SevenZipArchive() {#SevenZipArchive--}
```
public SevenZipArchive()
```


[SevenZipArchive](../../com.aspose.zip/sevenziparchive) sınıfının yeni bir örneğini girişleri için isteğe bağlı ayarlarla başlatır.

Aşağıdaki örnek, tek bir dosyayı varsayılan ayarlarla nasıl sıkıştıracağınızı gösterir: Şifreleme olmadan LZMA sıkıştırması.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
try (SevenZipArchive archive = new SevenZipArchive()) {
archive.createEntry("data.bin", "file.dat");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

LZMA compression without encryption would be used.

### SevenZipArchive(SevenZipEntrySettings newEntrySettings) {#SevenZipArchive-com.aspose.zip.SevenZipEntrySettings-}
```
public SevenZipArchive(SevenZipEntrySettings newEntrySettings)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class with optional settings for its entries.

The following example shows how to compress a single file with default settings: LZMA compression without encryption.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         try (SevenZipArchive archive = new SevenZipArchive()) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | Yeni eklenen [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) öğeleri için kullanılan sıkıştırma ve şifreleme ayarları. Belirtilmezse, şifreleme olmadan LZMA sıkıştırması kullanılır. |

### SevenZipArchive(InputStream sourceStream) {#SevenZipArchive-java.io.InputStream-}
```
public SevenZipArchive(InputStream sourceStream)
```


Yeni bir [SevenZipArchive](../../com.aspose.zip/sevenziparchive) sınıfı örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new FileInputStream("archive.7z"))) {
archive.extractToDirectory("C:\\extracted");
} catch (FileNotFoundException ex) {
}
 
```

This constructor does not decompress any entry. See [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### SevenZipArchive(InputStream sourceStream, String password) {#SevenZipArchive-java.io.InputStream-java.lang.String-}
```
public SevenZipArchive(InputStream sourceStream, String password)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class and composes an entry list can be extracted from the archive.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new FileInputStream("archive.7z"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (FileNotFoundException ex) {
     }
 
```

Bu yapıcı, herhangi bir girişi açmaz. Açmak için [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceStream | java.io.InputStream | arşivin kaynağı |
| password | java.lang.String | Şifre çözme için isteğe bağlı parola. Dosya adları şifrelenmişse, bu parola bulunmalıdır. |

### SevenZipArchive(String path) {#SevenZipArchive-java.lang.String-}
```
public SevenZipArchive(String path)
```


Yeni bir [SevenZipArchive](../../com.aspose.zip/sevenziparchive) sınıfı örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.extractToDirectory("C:\\extracted");
} catch (FileNotFoundException ex) {
}
 
```

This constructor does not decompress any entry. See [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the fully qualified or the relative path to the archive file |

### SevenZipArchive(String path, String password) {#SevenZipArchive-java.lang.String-java.lang.String-}
```
public SevenZipArchive(String path, String password)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class and composes an entry list can be extracted from the archive.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (FileNotFoundException ex) {
     }
 
```

Bu yapıcı, herhangi bir girişi açmaz. Açmak için [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | arşiv dosyasının tam nitelikli veya göreli yolu |
| password | java.lang.String | Şifre çözme için isteğe bağlı parola. Dosya adları şifrelenmişse, bu parola bulunmalıdır. |

### SevenZipArchive(InputStream sourceStream, SevenZipLoadOptions options) {#SevenZipArchive-java.io.InputStream-com.aspose.zip.SevenZipLoadOptions-}
```
public SevenZipArchive(InputStream sourceStream, SevenZipLoadOptions options)
```


Yeni bir [SevenZipArchive](../../com.aspose.zip/sevenziparchive) sınıfı örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

Şifreli bir arşivi çıkarın. İşlemin 60 saniyeye kadar sürmesine izin verin, bu süreden sonra iptal edin.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
SevenZipLoadOptions options = new SevenZipLoadOptions();
options.setDecryptionPassword("Top$ecr3t");
options.setCancellationFlag(cf);
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
try (SevenZipArchive a = new SevenZipArchive(new FileInputStream("archive.7z"), options)) {
a.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| options | [SevenZipLoadOptions](../../com.aspose.zip/sevenziploadoptions) | Options to load existing archive with.

This constructor does not decompress any entry. See [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) method for decompressing. |

### SevenZipArchive(String path, SevenZipLoadOptions options) {#SevenZipArchive-java.lang.String-com.aspose.zip.SevenZipLoadOptions-}
```
public SevenZipArchive(String path, SevenZipLoadOptions options)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class and composes an entry list can be extracted from the archive.

Extract an encrypted archive. Allow up to 60 seconds to proceed, cancel after that period.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         SevenZipLoadOptions options = new SevenZipLoadOptions();
         options.setDecryptionPassword("Top$ecr3t");
         options.setCancellationFlag(cf);
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         try (SevenZipArchive a = new SevenZipArchive(new FileInputStream("archive.7z"), options)) {
             a.extractToDirectory("C:\\extracted");
         } catch (IOException ex) {
         }
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | Arşiv dosyasına tam nitelikli veya göreli yol. |
|  | options | [SevenZipLoadOptions](../../com.aspose.zip/sevenziploadoptions) | Mevcut arşivi yüklemek için seçenekler. |

Bu yapıcı, herhangi bir girişi açmaz. Açmak için [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) yöntemine bakın. |

### SevenZipArchive(String[] parts) {#SevenZipArchive-java.lang.String---}
```
public SevenZipArchive(String[] parts)
```


Çok bölümlü 7z arşivinden yeni bir [SevenZipArchive](../../com.aspose.zip/sevenziparchive) sınıfı örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new String[] { "multi.7z.001", "multi.7z.002", "multi.7z.003" } )) {
archive.extractToDirectory("C:\\extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| parts | java.lang.String[] | paths to each segment of multi-volume 7z archive respecting order |

### SevenZipArchive(String[] parts, String password) {#SevenZipArchive-java.lang.String---java.lang.String-}
```
public SevenZipArchive(String[] parts, String password)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class from multi-volume 7z archive and composes an entry list can be extracted from the archive.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new String[] { "multi.7z.001", "multi.7z.002", "multi.7z.003" } )) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bölümler | java.lang.String[] | çok bölümlü 7z arşivinin her segmentine ait yollar, sıralamayı koruyarak |
| password | java.lang.String | Şifre çözme için isteğe bağlı parola. Dosya adları şifrelenmişse, bu parola bulunmalıdır. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final SevenZipArchive createEntries(File directory)
```


Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler.

```

``````

try (SevenZipArchive archive = new SevenZipArchive()) {
File folder = new File("C:\\folder");
archive.createEntries(folder);
archive.save("folder.7z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |

**Returns:**
[SevenZipArchive](../../com.aspose.zip/sevenziparchive) - the archive with entries composed
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final SevenZipArchive createEntries(File directory, boolean includeRootDirectory)
```


Adds to the archive all files and directories recursively in the directory given.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive()) {
         File folder = new File("C:\\folder");
         archive.createEntries(folder);
         archive.save("folder.7z");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| directory | java.io.File | sıkıştırılacak dizin |
| includeRootDirectory | boolean | kök dizini kendisini dahil edip etmeyeceğini gösterir |

**Returns:**
[SevenZipArchive](../../com.aspose.zip/sevenziparchive) - the archive with entries composed
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final SevenZipArchive createEntries(String sourceDirectory)
```


Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler.

LZMA sıkıştırmasıyla 7z arşivi oluşturun.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntries("C:\\folder");
archive.save("folder.7z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |

**Returns:**
[SevenZipArchive](../../com.aspose.zip/sevenziparchive) - the archive with entries composed
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final SevenZipArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Adds to the archive all files and directories recursively in the directory given.

Compose 7z archive with LZMA compression.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
         archive.createEntries("C:\\folder");
         archive.save("folder.7z");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceDirectory | java.lang.String | sıkıştırılacak dizin |
| includeRootDirectory | boolean | kök dizini kendisini dahil edip etmeyeceğini gösterir |

**Returns:**
[SevenZipArchive](../../com.aspose.zip/sevenziparchive) - the archive with entries composed
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final SevenZipArchiveEntry createEntry(String name, File file)
```


Arşiv içinde tek bir giriş oluşturur.

Her biri farklı şifrelerle şifrelenmiş girişlerle arşiv oluşturun.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
File fi1 = new File("data1.bin");
File fi2 = new File("data2.bin");
File fi3 = new File("data3.bin");

try (SevenZipArchive archive = new SevenZipArchive()) {
archive.createEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
archive.createEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
archive.createEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file to be compressed |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final SevenZipArchiveEntry createEntry(String name, File file, boolean openImmediately)
```


Creates a single entry within the archive.

Compose archive with entries encrypted with different passwords each.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         File fi1 = new File("data1.bin");
         File fi2 = new File("data2.bin");
         File fi3 = new File("data3.bin");

         try (SevenZipArchive archive = new SevenZipArchive()) {
             archive.createEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
             archive.createEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
             archive.createEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

Giriş adı yalnızca `name` parametresi içinde ayarlanır. `file` parametresinde verilen dosya adı giriş adını etkilemez.

`openImmediately` parametresiyle dosya hemen açılırsa, arşiv kaydedilene kadar engellenir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | girişin adı |
| dosya | java.io.File | sıkıştırılacak dosyanın meta verileri |
| openImmediately | boolean | doğru, dosyayı hemen açmak için, aksi takdirde arşiv kaydedilirken dosyayı açar |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, File file, boolean openImmediately, SevenZipEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.SevenZipEntrySettings-}
```
public final SevenZipArchiveEntry createEntry(String name, File file, boolean openImmediately, SevenZipEntrySettings newEntrySettings)
```


Arşiv içinde tek bir giriş oluşturur.

Her biri farklı şifrelerle şifrelenmiş girişlerle arşiv oluşturun.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
File fi1 = new File("data1.bin");
File fi2 = new File("data2.bin");
File fi3 = new File("data3.bin");

try (SevenZipArchive archive = new SevenZipArchive()) {
archive.createEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
archive.createEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
archive.createEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | compression and encryption settings used for added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) item. Individual compression settings is ignored in case of solid compression, see `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final SevenZipArchiveEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

Compose 7z archive with LZMA compression and encryption of all entries.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings(), new SevenZipAESEncryptionSettings("p@s$")))) {
         archive.createEntry("data.bin", new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF} ));
         archive.save("archive.7z");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | girişin adı |
| source | java.io.InputStream | girdi için giriş akışı |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.SevenZipEntrySettings-}
```
public final SevenZipArchiveEntry createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings)
```


Arşiv içinde tek bir giriş oluşturur.

Tüm girişlerin LZMA sıkıştırması ve şifrelemesiyle 7z arşivi oluşturun.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings(), new SevenZipAESEncryptionSettings("p@s$")))) {
archive.createEntry("data.bin", new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF} ));
archive.save("archive.7z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | compression and encryption settings used for added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) item. Individual compression settings is ignored in case of solid compression, see `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings, File file) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.SevenZipEntrySettings-java.io.File-}
```
public final SevenZipArchiveEntry createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings, File file)
```


Creates a single entry within the archive.

Compose archive with LZMA compressed encrypted entry.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         try (SevenZipArchive archive = new SevenZipArchive()) {
             archive.createEntry("entry1.bin", new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF}), new SevenZipEntrySettings(new SevenZipLZMACompressionSettings(), new SevenZipAESEncryptionSettings("test1")), new File("data1.bin"));
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

Giriş adı yalnızca `name` parametresi içinde ayarlanır. `file` parametresinde verilen dosya adı giriş adını etkilemez.

`file` bir dizine referans gösterebilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | girişin adı |
| source | java.io.InputStream | girdi için giriş akışı |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | eklenen [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) öğesi için kullanılan sıkıştırma ve şifreleme ayarları. Katı sıkıştırma durumunda bireysel sıkıştırma ayarları göz ardı edilir, bakınız `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |
| dosya | java.io.File | sıkıştırılacak dosya veya klasörün meta verileri |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final SevenZipArchiveEntry createEntry(String name, String path)
```


Arşiv içinde tek bir giriş oluşturur.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntry("data.bin", "file.dat");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | the fully qualified name of the new file, or the relative file name to be compressed |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final SevenZipArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Creates a single entry within the archive.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

Giriş adı yalnızca `name` parametresi içinde ayarlanır. `path` parametresinde verilen dosya adı giriş adını etkilemez.

`openImmediately` parametresiyle dosya hemen açılırsa, arşiv kaydedilene kadar engellenir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | girişin adı |
| path | java.lang.String | yeni dosyanın tam nitelikli adı veya sıkıştırılacak göreli dosya adı |
| openImmediately | boolean | doğru, dosyayı hemen açmak için, aksi takdirde arşiv kaydedilirken dosyayı açar |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, String path, boolean openImmediately, SevenZipEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.SevenZipEntrySettings-}
```
public final SevenZipArchiveEntry createEntry(String name, String path, boolean openImmediately, SevenZipEntrySettings newEntrySettings)
```


Arşiv içinde tek bir giriş oluşturur.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntry("data.bin", "file.dat");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | the fully qualified name of the new file, or the relative file name to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | compression and encryption settings used for added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) item. Individual compression settings is ignored in case of solid compression, see `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Zip entry instance
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--}
```
public final SevenZipArchiveEntry createEntry(String name, Supplier<InputStream> streamProvider)
```


Create a single entry within the archive.

Compose archive with LZMA2 compressed encrypted entry.

```

``````

 System.Func&lt;Stream&gt; provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
 using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
 {
     using (var archive = new SevenZipArchive())
     {
         archive.CreateEntry("entry1.bin", provider, new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1"))); 
         archive.Save(sevenZipFile);
     }
 }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Girişin adı. |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | Giriş akışı sağlayan yöntem. |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - SevenZip entry instance.
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, SevenZipEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.SevenZipEntrySettings-}
```
public final SevenZipArchiveEntry createEntry(String name, Supplier<InputStream> streamProvider, SevenZipEntrySettings newEntrySettings)
```


Arşiv içinde tek bir giriş oluştur.

LZMA2 sıkıştırmalı şifreli giriş ile arşivi oluştur.

```

``````

System.Func&lt;Stream&gt; provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
using (var archive = new SevenZipArchive())
{
archive.CreateEntry("entry1.bin", provider, new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
archive.Save(sevenZipFile);
}
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | The method providing input stream for the entry. |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | Compression and encryption settings used for added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) item. Individual compression settings is ignored in case of solid compression, see `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - SevenZip entry instance.
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | çıkarılan dosyaların yerleştirileceği dizine giden yol. |

Dizin mevcut değilse, oluşturulacaktır |

### extractToDirectory(String destinationDirectory, String password) {#extractToDirectory-java.lang.String-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory, String password)
```


Arşivdeki tüm dosyaları verilen dizine çıkarır.

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.extractToDirectory("C:\\extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in

If the directory does not exist, it will be created. |
| password | java.lang.String | optional password for content decryption.

`password` is used for content decryption only. If file names are encrypted provide password in [SevenZipArchive(String, String)](../../com.aspose.zip/sevenziparchive\#SevenZipArchive-String--String-) or [SevenZipArchive(java.io.InputStream, String)](../../com.aspose.zip/sevenziparchive\#SevenZipArchive-java.io.InputStream--String-) constructor. |

### getEntries() {#getEntries--}
```
public final List<SevenZipArchiveEntry> getEntries()
```


Gets entries of [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.SevenZipArchiveEntry&gt; - entries of [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) type constituting the archive
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the 7z archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the 7z archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final SevenZipEntrySettings getNewEntrySettings()
```


Compression and encryption settings used for newly added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) items.

**Returns:**
[SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) - compression and encryption settings used for newly added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) items
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves 7z archive to the stream provided.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (SevenZipArchive archive = new SevenZipArchive()) {
                 archive.createEntry("data", source);
                 archive.save(sevenZipFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| output | java.io.OutputStream | hedef akışı |

### save(OutputStream output, SevenZipArchiveSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.SevenZipArchiveSaveOptions-}
```
public final void save(OutputStream output, SevenZipArchiveSaveOptions saveOptions)
```


7z arşivini sağlanan akışa kaydeder.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (SevenZipArchive archive = new SevenZipArchive()) {
archive.createEntry("data", source);
archive.save(sevenZipFile);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream |
| saveOptions | [SevenZipArchiveSaveOptions](../../com.aspose.zip/sevenziparchivesaveoptions) | Options for archive saving. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to a destination file provided.

```

``````

  using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
  {
     using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
     {
        archive.CreateEntry("data", source);
        archive.Save("archive.7z");
     }
  }
  
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | destinationFileName | java.lang.String | Oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |

Bir arşivi yüklendiği aynı yola kaydetmek mümkündür. Ancak, bu yöntem geçici bir dosyaya kopyalama yaptığı için önerilmez. |

### save(String destinationFileName, SevenZipArchiveSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.SevenZipArchiveSaveOptions-}
```
public final void save(String destinationFileName, SevenZipArchiveSaveOptions saveOptions)
```


Arşivi sağlanan hedef dosyaya kaydeder.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntry("data", source);
archive.save("archive.7z");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |
| saveOptions | [SevenZipArchiveSaveOptions](../../com.aspose.zip/sevenziparchivesaveoptions) | Options for archive saving.

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file. |

### saveSplit(String destinationDirectory, SplitSevenZipArchiveSaveOptions options) {#saveSplit-java.lang.String-com.aspose.zip.SplitSevenZipArchiveSaveOptions-}
```
public final void saveSplit(String destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```


Saves multi-volume archive to destination directory provided.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive()) {
         archive.createEntry("entry.bin", "data.bin");
         archive.saveSplit("C:\\Folder", new SplitSevenZipArchiveSaveOptions("volume", 65536));
     }
 
```

Bu yöntem, birkaç `(n)` dosyası filename.7z.001, filename.7z.002, ..., filename.7z.(n) oluşturur.

Mevcut arşivi çok bölümlü yapamaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationDirectory | java.lang.String | arşiv segmentlerinin oluşturulacağı dizinin yolu |
| options | [SplitSevenZipArchiveSaveOptions](../../com.aspose.zip/splitsevenziparchivesaveoptions) | dosya adı dahil olmak üzere arşiv kaydetme seçenekleri |

