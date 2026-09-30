---
title: "TarArchive"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bu sınıf bir tar arşiv dosyasını temsil eder."
type: docs
weight: 125
url: /tr/java/com.aspose.zip/tararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class TarArchive implements IArchive, AutoCloseable
```

Bu sınıf bir tar arşiv dosyasını temsil eder. Tar arşivlerini oluşturmak, çıkarmak veya güncellemek için kullanın.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [TarArchive()](#TarArchive--) | [TarArchive](../../com.aspose.zip/tararchive) sınıfının yeni bir örneğini başlatır. |
| [TarArchive(InputStream sourceStream)](#TarArchive-java.io.InputStream-) | Yeni bir [Archive](../../com.aspose.zip/archive) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [TarArchive(String path)](#TarArchive-java.lang.String-) | [TarArchive](../../com.aspose.zip/tararchive) sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
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
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Arşiv içinde tek bir giriş oluşturur. |
| [createEntry(String name, InputStream source, File file)](#createEntry-java.lang.String-java.io.InputStream-java.io.File-) | Arşiv içinde tek bir giriş oluşturur. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Arşiv içinde tek bir giriş oluşturur. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Arşiv içinde tek bir giriş oluşturur. |
| [deleteEntry(TarEntry entry)](#deleteEntry-com.aspose.zip.TarEntry-) | Giriş listesinden belirli bir girdinin ilk oluşumunu kaldırır. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Giriş listesinden girdiyi indeksine göre kaldırır. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Arşivdeki tüm dosyaları verilen dizine çıkarır. |
| [fromGZip(InputStream source)](#fromGZip-java.io.InputStream-) | Sağlanan gzip arşivini çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur. |
| [fromGZip(String path)](#fromGZip-java.lang.String-) | Sağlanan gzip arşivini çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur. |
| [fromLZ4(InputStream source)](#fromLZ4-java.io.InputStream-) | Sağlanan LZ4 arşivini çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur. |
| [fromLZ4(String path)](#fromLZ4-java.lang.String-) | Sağlanan LZ4 arşivini çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur. |
| [fromLZMA(InputStream source)](#fromLZMA-java.io.InputStream-) | Sağlanan LZMA arşivini çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur. |
| [fromLZMA(String path)](#fromLZMA-java.lang.String-) | Sağlanan LZMA arşivini çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur. |
| [fromLZip(InputStream source)](#fromLZip-java.io.InputStream-) | Sağlanan lzip arşivini çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur. |
| [fromLZip(String path)](#fromLZip-java.lang.String-) | Sağlanan lzip arşivini çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur. |
| [fromXz(InputStream source)](#fromXz-java.io.InputStream-) | Sağlanan xz formatındaki arşivi çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur. |
| [fromXz(String path)](#fromXz-java.lang.String-) | Sağlanan xz formatındaki arşivi çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur. |
| [fromZ(InputStream source)](#fromZ-java.io.InputStream-) | Sağlanan Z formatındaki arşivi çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur. |
| [fromZ(String path)](#fromZ-java.lang.String-) | Sağlanan Z formatındaki arşivi çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur. |
| [fromZstandard(InputStream source)](#fromZstandard-java.io.InputStream-) | Sağlanan Zstandard arşivini çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur. |
| [fromZstandard(String path)](#fromZstandard-java.lang.String-) | Sağlanan Zstandard arşivini çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur. |
| [getEntries()](#getEntries--) | Arşivi oluşturan [TarEntry](../../com.aspose.zip/tarentry) türündeki girişleri alır. |
| [getFileEntries()](#getFileEntries--) | Tar arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) tipindeki girişleri alır. |
| [getFormat()](#getFormat--) | Arşiv biçimini alır. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Sağlanan akışa arşivi kaydeder. |
| [save(OutputStream output, TarFormat format)](#save-java.io.OutputStream-com.aspose.zip.TarFormat-) | Sağlanan akışa arşivi kaydeder. |
| [save(String destinationFileName)](#save-java.lang.String-) | Sağlanan hedef dosyaya arşivi kaydeder. |
| [save(String destinationFileName, TarFormat format)](#save-java.lang.String-com.aspose.zip.TarFormat-) | Sağlanan hedef dosyaya arşivi kaydeder. |
| [saveGzipped(OutputStream output)](#saveGzipped-java.io.OutputStream-) | Arşivi gzip sıkıştırmasıyla akışa kaydeder. |
| [saveGzipped(OutputStream output, TarFormat format)](#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | Arşivi gzip sıkıştırmasıyla akışa kaydeder. |
| [saveGzipped(String path)](#saveGzipped-java.lang.String-) | Arşivi gzip sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveGzipped(String path, TarFormat format)](#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-) | Arşivi gzip sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveLZ4Compressed(OutputStream output)](#saveLZ4Compressed-java.io.OutputStream-) | Arşivi LZ4 sıkıştırmasıyla akışa kaydeder. |
| [saveLZ4Compressed(OutputStream output, TarFormat format)](#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Arşivi LZ4 sıkıştırmasıyla akışa kaydeder. |
| [saveLZ4Compressed(String path)](#saveLZ4Compressed-java.lang.String-) | Arşivi LZ4 sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveLZ4Compressed(String path, TarFormat format)](#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-) | Arşivi LZ4 sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveLZMACompressed(OutputStream output)](#saveLZMACompressed-java.io.OutputStream-) | Arşivi LZMA sıkıştırmasıyla akışa kaydeder. |
| [saveLZMACompressed(OutputStream output, TarFormat format)](#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Arşivi LZMA sıkıştırmasıyla akışa kaydeder. |
| [saveLZMACompressed(String path)](#saveLZMACompressed-java.lang.String-) | Arşivi lzma sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveLZMACompressed(String path, TarFormat format)](#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-) | Arşivi lzma sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveLzipped(OutputStream output)](#saveLzipped-java.io.OutputStream-) | Arşivi lzip sıkıştırmasıyla akışa kaydeder. |
| [saveLzipped(OutputStream output, TarFormat format)](#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | Arşivi lzip sıkıştırmasıyla akışa kaydeder. |
| [saveLzipped(String path)](#saveLzipped-java.lang.String-) | Arşivi lzip sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveLzipped(String path, TarFormat format)](#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-) | Arşivi lzip sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveXzCompressed(OutputStream output)](#saveXzCompressed-java.io.OutputStream-) | Arşivi xz sıkıştırmasıyla akışa kaydeder. |
| [saveXzCompressed(OutputStream output, TarFormat format)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Arşivi xz sıkıştırmasıyla akışa kaydeder. |
| [saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | Arşivi xz sıkıştırmasıyla akışa kaydeder. |
| [saveXzCompressed(String path)](#saveXzCompressed-java.lang.String-) | Arşivi xz sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveXzCompressed(String path, TarFormat format)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-) | Arşivi xz sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | Arşivi xz sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveZCompressed(OutputStream output)](#saveZCompressed-java.io.OutputStream-) | Arşivi Z sıkıştırmasıyla akışa kaydeder. |
| [saveZCompressed(OutputStream output, TarFormat format)](#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Arşivi Z sıkıştırmasıyla akışa kaydeder. |
| [saveZCompressed(String path)](#saveZCompressed-java.lang.String-) | Arşivi Z sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveZCompressed(String path, TarFormat format)](#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-) | Arşivi Z sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveZstandard(OutputStream output)](#saveZstandard-java.io.OutputStream-) | Arşivi Zstandard sıkıştırmasıyla akışa kaydeder. |
| [saveZstandard(OutputStream output, TarFormat format)](#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-) | Arşivi Zstandard sıkıştırmasıyla akışa kaydeder. |
| [saveZstandard(String path)](#saveZstandard-java.lang.String-) | Arşivi Zstandard sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveZstandard(String path, TarFormat format)](#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-) | Arşivi Zstandard sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
### TarArchive() {#TarArchive--}
```
public TarArchive()
```


[TarArchive](../../com.aspose.zip/tararchive) sınıfının yeni bir örneğini başlatır.

Aşağıdaki örnek bir dosyanın nasıl sıkıştırılacağını gösterir.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, \"data.bin\");
archive.save(\"archive.tar\");
}
 
```



### TarArchive(InputStream sourceStream) {#TarArchive-java.io.InputStream-}
```
public TarArchive(InputStream sourceStream)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (TarArchive archive = new TarArchive(new FileInputStream("archive.tar"))) {
             archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Bu yapıcı herhangi bir girişi açmaz. Açmak için [TarEntry.open()](../../com.aspose.zip/tarentry\\#open--) metoduna bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceStream | java.io.InputStream | arşivin kaynağı |

### TarArchive(String path) {#TarArchive-java.lang.String-}
```
public TarArchive(String path)
```


[TarArchive](../../com.aspose.zip/tararchive) sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

Aşağıdaki örnek, tüm girdileri bir dizine nasıl çıkarılacağını gösterir.

```

``````

try (TarArchive archive = new TarArchive(\"archive.tar\")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [TarEntry.open()](../../com.aspose.zip/tarentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final TarArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| directory | java.io.File | sıkıştırılacak dizin |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final TarArchive createEntries(File directory, boolean includeRootDirectory)
```


Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler.

```

``````

try (FileOutputStream tarFile = new FileOutputStream(\"archive.tar\")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final TarArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceDirectory | java.lang.String | sıkıştırılacak dizin |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final TarArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler.

```

``````

try (FileOutputStream tarFile = new FileOutputStream(\"archive.tar\")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final TarEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     File fi = new File("data.bin");
     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("data.bin", fi);
         archive.save(tarFile);
     }
 
```

Giriş adı yalnızca `name` parametresi içinde ayarlanır. `file` parametresinde verilen dosya adı giriş adını etkilemez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | girişin adı |
| dosya | java.io.File | sıkıştırılacak dosya veya klasörün meta verileri |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final TarEntry createEntry(String name, File file, boolean openImmediately)
```


Arşiv içinde tek bir giriş oluşturur.

```

``````

File fi = new File(\"data.bin\");
try (TarArchive archive = new TarArchive()) {
archive.createEntry(\"data.bin\", fi);
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final TarEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("bytes", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
         archive.save(tarFile);
     }
 
```

Giriş adı yalnızca `name` parametresi içinde ayarlanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | girişin adı |
| source | java.io.InputStream | girdi için giriş akışı |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source, File file) {#createEntry-java.lang.String-java.io.InputStream-java.io.File-}
```
public final TarEntry createEntry(String name, InputStream source, File file)
```


Arşiv içinde tek bir giriş oluşturur.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(\"bytes\", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| file | java.io.File | the metadata of file or folder to be compressed |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final TarEntry createEntry(String name, String path)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
             archive.createEntry(first.bin, "data.bin");
             archive.save(outputTarFile);
     }
 
```

Giriş adı yalnızca `name` parametresi içinde ayarlanır. `path` parametresinde verilen dosya adı giriş adını etkilemez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | girişin adı |
| path | java.lang.String | sıkıştırılacak dosyanın yolu |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final TarEntry createEntry(String name, String path, boolean openImmediately)
```


Arşiv içinde tek bir giriş oluşturur.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, \"data.bin\");
archive.save(outputTarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | path to file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### deleteEntry(TarEntry entry) {#deleteEntry-com.aspose.zip.TarEntry-}
```
public final TarArchive deleteEntry(TarEntry entry)
```


Removes the first occurrence of a specific entry from the entry list.

Here is how you can remove all entries except the last one:

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         while (archive.getEntries().size() > 1)
             archive.deleteEntry(archive.getEntries().get_Item(0));
         archive.save(outputTarFile);
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| entry | [TarEntry](../../com.aspose.zip/tarentry) | giriş listesinden kaldırılacak giriş |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final TarArchive deleteEntry(int entryIndex)
```


Giriş listesinden girdiyi indeksine göre kaldırır.

```

``````

try (TarArchive archive = new TarArchive("two_files.tar")) {
archive.deleteEntry(0);
archive.save("single_file.tar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | int | the zero-based index of the entry to remove |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

Dizin mevcut değilse, oluşturulacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationDirectory | java.lang.String | çıkarılan dosyaların yerleştirileceği dizinin yolu |

### fromGZip(InputStream source) {#fromGZip-java.io.InputStream-}
```
public static TarArchive fromGZip(InputStream source)
```


Sağlanan gzip arşivini çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur.

Önemli: gzip arşivi bu yöntem içinde tamamen çıkarılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

GZip çıkarma akışı, sıkıştırma algoritmasının doğası gereği arama yapılabilir değildir. Tar arşivi, rastgele bir kaydı çıkarmak için bir kolaylık sağlar, bu yüzden altyapıda arama yapılabilir bir akış kullanmak zorundadır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | java.io.InputStream | arşivin kaynağı. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromGZip(String path) {#fromGZip-java.lang.String-}
```
public static TarArchive fromGZip(String path)
```


Sağlanan gzip arşivini çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur.

Önemli: gzip arşivi bu yöntem içinde tamamen çıkarılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

GZip çıkarma akışı, sıkıştırma algoritmasının doğası gereği arama yapılabilir değildir. Tar arşivi, rastgele bir kaydı çıkarmak için bir kolaylık sağlar, bu yüzden altyapıda arama yapılabilir bir akış kullanmak zorundadır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | arşiv dosyasının yolu. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(InputStream source) {#fromLZ4-java.io.InputStream-}
```
public static TarArchive fromLZ4(InputStream source)
```


Sağlanan LZ4 arşivini çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur.

Önemli: LZ4 arşivi bu yöntem içinde tamamen çıkarılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | source | java.io.InputStream | Arşivin kaynağı. |

LZ4 çıkarma akışı, sıkıştırma algoritmasının doğası gereği arama yapılabilir değildir. Tar arşivi, rastgele bir kaydı çıkarmak için bir kolaylık sağlar, bu yüzden altyapıda arama yapılabilir bir akış kullanmak zorundadır. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(String path) {#fromLZ4-java.lang.String-}
```
public static TarArchive fromLZ4(String path)
```


Sağlanan LZ4 arşivini çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur.

Önemli: LZ4 arşivi bu yöntem içinde tamamen çıkarılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | path | java.lang.String | Arşiv dosyasının yolu. |

LZ4 çıkarma akışı, sıkıştırma algoritmasının doğası gereği arama yapılabilir değildir. Tar arşivi, rastgele bir kaydı çıkarmak için bir kolaylık sağlar, bu yüzden altyapıda arama yapılabilir bir akış kullanmak zorundadır. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(InputStream source) {#fromLZMA-java.io.InputStream-}
```
public static TarArchive fromLZMA(InputStream source)
```


Sağlanan LZMA arşivini çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur.

Önemli: LZMA arşivi bu yöntem içinde tamamen çıkarılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

LZMA çıkarma akışı, sıkıştırma algoritmasının doğası gereği arama yapılabilir değildir. Tar arşivi, rastgele bir kaydı çıkarmak için bir kolaylık sağlar, bu yüzden altyapıda arama yapılabilir bir akış kullanmak zorundadır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | java.io.InputStream | arşivin kaynağı |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(String path) {#fromLZMA-java.lang.String-}
```
public static TarArchive fromLZMA(String path)
```


Sağlanan LZMA arşivini çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur.

Önemli: LZMA arşivi bu yöntem içinde tamamen çıkarılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

LZMA çıkarma akışı, sıkıştırma algoritmasının doğası gereği arama yapılabilir değildir. Tar arşivi, rastgele bir kaydı çıkarmak için bir kolaylık sağlar, bu yüzden altyapıda arama yapılabilir bir akış kullanmak zorundadır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | arşiv dosyasının yolu |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(InputStream source) {#fromLZip-java.io.InputStream-}
```
public static TarArchive fromLZip(InputStream source)
```


Sağlanan lzip arşivini çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur.

Önemli: lzip arşivi bu yöntem içinde tamamen çıkarılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

Lzip çıkarma akışı, sıkıştırma algoritmasının doğası gereği arama yapılabilir değildir. Tar arşivi, rastgele bir kaydı çıkarmak için bir kolaylık sağlar, bu yüzden altyapıda arama yapılabilir bir akış kullanmak zorundadır

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | java.io.InputStream | arşivin kaynağı. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(String path) {#fromLZip-java.lang.String-}
```
public static TarArchive fromLZip(String path)
```


Sağlanan lzip arşivini çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur.

Önemli: lzip arşivi bu yöntem içinde tamamen çıkarılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

Lzip çıkarma akışı, sıkıştırma algoritmasının doğası gereği arama yapılabilir değildir. Tar arşivi, rastgele bir kaydı çıkarmak için bir kolaylık sağlar, bu yüzden altyapıda arama yapılabilir bir akış kullanmak zorundadır

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | arşiv dosyasının yolu. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(InputStream source) {#fromXz-java.io.InputStream-}
```
public static TarArchive fromXz(InputStream source)
```


Sağlanan xz formatındaki arşivi çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur.

Önemli: xz arşivi bu yöntem içinde tamamen çıkarılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

Tar arşivi, rastgele bir kaydı çıkarmak için bir kolaylık sağlar, bu yüzden altyapıda arama yapılabilir bir akış kullanmak zorundadır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | java.io.InputStream | arşivin kaynağı |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(String path) {#fromXz-java.lang.String-}
```
public static TarArchive fromXz(String path)
```


Sağlanan xz formatındaki arşivi çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur.

Önemli: xz arşivi bu yöntem içinde tamamen çıkarılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

Tar arşivi, rastgele bir kaydı çıkarmak için bir kolaylık sağlar, bu yüzden altyapıda arama yapılabilir bir akış kullanmak zorundadır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | arşiv dosyasının yolu |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(InputStream source) {#fromZ-java.io.InputStream-}
```
public static TarArchive fromZ(InputStream source)
```


Sağlanan Z formatındaki arşivi çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur.

Önemli: Z arşivi bu yöntem içinde tamamen çıkarılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | java.io.InputStream | arşivin kaynağı |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(String path) {#fromZ-java.lang.String-}
```
public static TarArchive fromZ(String path)
```


Sağlanan Z formatındaki arşivi çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur.

Önemli: Z arşivi bu yöntem içinde tamamen çıkarılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | arşiv dosyasının yolu |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(InputStream source) {#fromZstandard-java.io.InputStream-}
```
public static TarArchive fromZstandard(InputStream source)
```


Sağlanan Zstandard arşivini çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur.

Önemli: Zstandard arşivi bu yöntem içinde tamamen çıkarılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | java.io.InputStream | arşivin kaynağı |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(String path) {#fromZstandard-java.lang.String-}
```
public static TarArchive fromZstandard(String path)
```


Sağlanan Zstandard arşivini çıkarır ve çıkarılan verilerden [TarArchive](../../com.aspose.zip/tararchive) oluşturur.

Önemli: Zstandard arşivi bu yöntem içinde tamamen çıkarılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | arşiv dosyasının yolu |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### getEntries() {#getEntries--}
```
public final List<TarEntry> getEntries()
```


Arşivi oluşturan [TarEntry](../../com.aspose.zip/tarentry) türündeki girişleri alır.

**Returns:**
java.util.List&lt;com.aspose.zip.TarEntry&gt; - arşivi oluşturan [TarEntry](../../com.aspose.zip/tarentry) tipindeki girişler
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Tar arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) tipindeki girişleri alır.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - tar arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) tipindeki girişler
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Arşiv biçimini alır.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Sağlanan akışa arşivi kaydeder.

```

``````

try (FileOutputStream tarFile = new FileOutputStream(\"archive.tar\")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### save(OutputStream output, TarFormat format) {#save-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void save(OutputStream output, TarFormat format)
```


Saves archive to the stream provided.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry1", "data.bin");
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | output | java.io.OutputStream | hedef akış. |

`output` yazılabilir olmalıdır |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar başlık formatını tanımlar. Null değeri mümkün olduğunda USTar olarak ele alınacaktır. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Sağlanan hedef dosyaya arşivi kaydeder.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save("myarchive.tar");
}
 
```

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### save(String destinationFileName, TarFormat format) {#save-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void save(String destinationFileName, TarFormat format)
```


Saves archive to the destination file provided.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("myarchive.tar");
     }
 
```

Bir arşivi yüklendiği aynı yola kaydetmek mümkündür. Ancak, bu yöntem geçici bir dosyaya kopyalama yaptığı için önerilmez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationFileName | java.lang.String | oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar başlık formatını tanımlar. Null değeri mümkün olduğunda USTar olarak ele alınacaktır. |

### saveGzipped(OutputStream output) {#saveGzipped-java.io.OutputStream-}
```
public final void saveGzipped(OutputStream output)
```


Arşivi gzip sıkıştırmasıyla akışa kaydeder.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped(result);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveGzipped(OutputStream output, TarFormat format) {#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with gzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveGzipped(result);
             }
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | output | java.io.OutputStream | hedef akış. |

`output` yazılabilir olmalıdır |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar başlık formatını tanımlar. Null değeri mümkün olduğunda USTar olarak ele alınacaktır. |

### saveGzipped(String path) {#saveGzipped-java.lang.String-}
```
public final void saveGzipped(String path)
```


Arşivi gzip sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped("result.tar.gz");
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveGzipped(String path, TarFormat format) {#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(String path, TarFormat format)
```


Saves archive to the file by path with gzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveGzipped("result.tar.gz");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar başlık formatını tanımlar. Null değeri mümkün olduğunda USTar olarak ele alınacaktır. |

### saveLZ4Compressed(OutputStream output) {#saveLZ4Compressed-java.io.OutputStream-}
```
public final void saveLZ4Compressed(OutputStream output)
```


Arşivi LZ4 sıkıştırmasıyla akışa kaydeder.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | Destination stream. |

### saveLZ4Compressed(OutputStream output, TarFormat format) {#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZ4 compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZ4Compressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| output | java.io.OutputStream | Hedef akış. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Tar başlık formatını tanımlar. Boş değer mümkün olduğunda USTar olarak kabul edilecektir. |

### saveLZ4Compressed(String path) {#saveLZ4Compressed-java.lang.String-}
```
public final void saveLZ4Compressed(String path)
```


Arşivi LZ4 sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed("result.tar.lz4");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### saveLZ4Compressed(String path, TarFormat format) {#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(String path, TarFormat format)
```


Saves archive to the file by path with LZ4 compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZ4Compressed("result.tar.lz4");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | Oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Tar başlık formatını tanımlar. Boş değer mümkün olduğunda USTar olarak kabul edilecektir. |

### saveLZMACompressed(OutputStream output) {#saveLZMACompressed-java.io.OutputStream-}
```
public final void saveLZMACompressed(OutputStream output)
```


Arşivi LZMA sıkıştırmasıyla akışa kaydeder.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed(result);
}
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveLZMACompressed(OutputStream output, TarFormat format) {#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZMA compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZMACompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```

Önemli: tar arşivi bu yöntemde oluşturulur ve ardından sıkıştırılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | output | java.io.OutputStream | hedef akış. |

`output` yazılabilir olmalıdır |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar başlık formatını tanımlar. Null değeri mümkün olduğunda USTar olarak ele alınacaktır. |

### saveLZMACompressed(String path) {#saveLZMACompressed-java.lang.String-}
```
public final void saveLZMACompressed(String path)
```


Arşivi lzma sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed("result.tar.lzma");
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLZMACompressed(String path, TarFormat format) {#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(String path, TarFormat format)
```


Saves archive to the file by path with lzma compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZMACompressed("result.tar.lzma");
         }
     } catch (IOException ex) {
     }
 
```

Önemli: tar arşivi bu yöntemde oluşturulur ve ardından sıkıştırılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar başlık formatını tanımlar. Null değeri mümkün olduğunda USTar olarak ele alınacaktır. |

### saveLzipped(OutputStream output) {#saveLzipped-java.io.OutputStream-}
```
public final void saveLzipped(OutputStream output)
```


Arşivi lzip sıkıştırmasıyla akışa kaydeder.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveLzipped(OutputStream output, TarFormat format) {#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with lzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLzipped(result, TarFormat.Gnu);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | output | java.io.OutputStream | hedef akış. |

`output` yazılabilir olmalıdır |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar başlık formatını tanımlar. Null değeri mümkün olduğunda USTar olarak ele alınacaktır. |

### saveLzipped(String path) {#saveLzipped-java.lang.String-}
```
public final void saveLzipped(String path)
```


Arşivi lzip sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped("result.tar.lz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLzipped(String path, TarFormat format) {#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(String path, TarFormat format)
```


Saves archive to the file by path with lzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLzipped("result.tar.lz", TarFormat.Gnu);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar başlık formatını tanımlar. Null değeri mümkün olduğunda USTar olarak ele alınacaktır. |

### saveXzCompressed(OutputStream output) {#saveXzCompressed-java.io.OutputStream-}
```
public final void saveXzCompressed(OutputStream output)
```


Arşivi xz sıkıştırmasıyla akışa kaydeder.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output`The stream must be writable |

### saveXzCompressed(OutputStream output, TarFormat format) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveXzCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | output | java.io.OutputStream | hedef akış. |

`output`Akış yazılabilir olmalıdır |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar başlık formatını tanımlar. Null değeri mümkün olduğunda USTar olarak ele alınacaktır. |

### saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)
```


Arşivi xz sıkıştırmasıyla akışa kaydeder.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output`The stream must be writable |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines the tar header format. Null value will be treated as USTar when possible |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | set of setting particular xz archive: dictionary size, block size, check type |

### saveXzCompressed(String path) {#saveXzCompressed-java.lang.String-}
```
public final void saveXzCompressed(String path)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |

### saveXzCompressed(String path, TarFormat format) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(String path, TarFormat format)
```


Arşivi xz sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed("result.tar.xz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines tar header format. Null value will be treated as USTar when possible |

### saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar başlık formatını tanımlar. Null değeri mümkün olduğunda USTar olarak ele alınacaktır. |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | belirli xz arşivi ayarları kümesi: sözlük boyutu, blok boyutu, kontrol türü |

### saveZCompressed(OutputStream output) {#saveZCompressed-java.io.OutputStream-}
```
public final void saveZCompressed(OutputStream output)
```


Arşivi Z sıkıştırmasıyla akışa kaydeder.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |

### saveZCompressed(OutputStream output, TarFormat format) {#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with Z compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| output | java.io.OutputStream | hedef akış |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar başlık formatını tanımlar. Null değeri mümkün olduğunda USTar olarak ele alınacaktır. |

### saveZCompressed(String path) {#saveZCompressed-java.lang.String-}
```
public final void saveZCompressed(String path)
```


Arşivi Z sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed("result.tar.Z");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZCompressed(String path, TarFormat format) {#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(String path, TarFormat format)
```


Saves archive to the file by path with Z compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZCompressed("result.tar.Z");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar başlık formatını tanımlar. Null değeri mümkün olduğunda USTar olarak ele alınacaktır. |

### saveZstandard(OutputStream output) {#saveZstandard-java.io.OutputStream-}
```
public final void saveZstandard(OutputStream output)
```


Arşivi Zstandard sıkıştırmasıyla akışa kaydeder.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveZstandard(OutputStream output, TarFormat format) {#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(OutputStream output, TarFormat format)
```


Saves archive to the stream with Zstandard compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZstandard(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | output | java.io.OutputStream | hedef akış. |

`output` yazılabilir olmalıdır |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar başlık formatını tanımlar. Null değeri mümkün olduğunda USTar olarak ele alınacaktır. |

### saveZstandard(String path) {#saveZstandard-java.lang.String-}
```
public final void saveZstandard(String path)
```


Arşivi Zstandard sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard("result.tar.zst");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZstandard(String path, TarFormat format) {#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(String path, TarFormat format)
```


Saves archive to the file by path with Zstandard compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZstandard("result.tar.zst");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar başlık formatını tanımlar. Null değeri mümkün olduğunda USTar olarak ele alınacaktır. |

