---
title: "CpioArchive"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bu sınıf cpio arşiv dosyasını temsil eder."
type: docs
weight: 57
url: /tr/java/com.aspose.zip/cpioarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class CpioArchive implements IArchive, AutoCloseable
```

Bu sınıf cpio arşiv dosyasını temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [CpioArchive()](#CpioArchive--) | Yeni bir [CpioArchive](../../com.aspose.zip/cpioarchive) sınıfının örneğini başlatır. |
| [CpioArchive(InputStream sourceStream)](#CpioArchive-java.io.InputStream-) | Yeni bir [CpioArchive](../../com.aspose.zip/cpioarchive) sınıfının örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [CpioArchive(String path)](#CpioArchive-java.lang.String-) | Yeni bir [CpioArchive](../../com.aspose.zip/cpioarchive) sınıfının örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
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
| [createEntry(String name, String sourcePath)](#createEntry-java.lang.String-java.lang.String-) | Arşiv içinde tek bir giriş oluşturur. |
| [createEntry(String name, String sourcePath, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Arşiv içinde tek bir giriş oluşturur. |
| [deleteEntry(CpioEntry entry)](#deleteEntry-com.aspose.zip.CpioEntry-) | Giriş listesinden belirli bir girdinin ilk oluşumunu kaldırır. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Giriş listesinden girdiyi indeksine göre kaldırır. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Arşivdeki tüm dosyaları verilen dizine çıkarır. |
| [getEntries()](#getEntries--) | Cpio arşivini oluşturan [CpioEntry](../../com.aspose.zip/cpioentry) türündeki girdileri alır. |
| [getFileEntries()](#getFileEntries--) | Cpio arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) türündeki girdileri alır. |
| [getFormat()](#getFormat--) | Arşiv biçimini alır. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Sağlanan akışa arşivi kaydeder. |
| [save(OutputStream output, CpioFormat cpioFormat)](#save-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Sağlanan akışa arşivi kaydeder. |
| [save(String destinationFileName)](#save-java.lang.String-) | Sağlanan hedef dosyaya arşivi kaydeder. |
| [save(String destinationFileName, CpioFormat cpioFormat)](#save-java.lang.String-com.aspose.zip.CpioFormat-) | Sağlanan hedef dosyaya arşivi kaydeder. |
| [saveGzipped(OutputStream output)](#saveGzipped-java.io.OutputStream-) | Arşivi gzip sıkıştırmasıyla akışa kaydeder. |
| [saveGzipped(OutputStream output, CpioFormat cpioFormat)](#saveGzipped-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Arşivi gzip sıkıştırmasıyla akışa kaydeder. |
| [saveGzipped(String path)](#saveGzipped-java.lang.String-) | Arşivi gzip sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveGzipped(String path, CpioFormat cpioFormat)](#saveGzipped-java.lang.String-com.aspose.zip.CpioFormat-) | Arşivi gzip sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveLZMACompressed(OutputStream output)](#saveLZMACompressed-java.io.OutputStream-) | Arşivi LZMA sıkıştırmasıyla akışa kaydeder. |
| [saveLZMACompressed(OutputStream output, CpioFormat cpioFormat)](#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Arşivi LZMA sıkıştırmasıyla akışa kaydeder. |
| [saveLZMACompressed(String path)](#saveLZMACompressed-java.lang.String-) | Arşivi lzma sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveLZMACompressed(String path, CpioFormat cpioFormat)](#saveLZMACompressed-java.lang.String-com.aspose.zip.CpioFormat-) | Arşivi lzma sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveLzipped(OutputStream output)](#saveLzipped-java.io.OutputStream-) | Arşivi lzip sıkıştırmasıyla akışa kaydeder. |
| [saveLzipped(OutputStream output, CpioFormat cpioFormat)](#saveLzipped-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Arşivi lzip sıkıştırmasıyla akışa kaydeder. |
| [saveLzipped(String path)](#saveLzipped-java.lang.String-) | Arşivi lzip sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveLzipped(String path, CpioFormat cpioFormat)](#saveLzipped-java.lang.String-com.aspose.zip.CpioFormat-) | Arşivi lzip sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveXzCompressed(OutputStream output)](#saveXzCompressed-java.io.OutputStream-) | Arşivi xz sıkıştırmasıyla akışa kaydeder. |
| [saveXzCompressed(OutputStream output, CpioFormat cpioFormat)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Arşivi xz sıkıştırmasıyla akışa kaydeder. |
| [saveXzCompressed(OutputStream output, CpioFormat cpioFormat, XzArchiveSettings settings)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-com.aspose.zip.XzArchiveSettings-) | Arşivi xz sıkıştırmasıyla akışa kaydeder. |
| [saveXzCompressed(String path)](#saveXzCompressed-java.lang.String-) | Arşivi xz sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveXzCompressed(String path, CpioFormat cpioFormat)](#saveXzCompressed-java.lang.String-com.aspose.zip.CpioFormat-) | Arşivi xz sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveXzCompressed(String path, CpioFormat cpioFormat, XzArchiveSettings settings)](#saveXzCompressed-java.lang.String-com.aspose.zip.CpioFormat-com.aspose.zip.XzArchiveSettings-) | Arşivi xz sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveZCompressed(OutputStream output)](#saveZCompressed-java.io.OutputStream-) | Arşivi Z sıkıştırmasıyla akışa kaydeder. |
| [saveZCompressed(OutputStream output, CpioFormat cpioFormat)](#saveZCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Arşivi Z sıkıştırmasıyla akışa kaydeder. |
| [saveZCompressed(String path)](#saveZCompressed-java.lang.String-) | Arşivi Z sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveZCompressed(String path, CpioFormat cpioFormat)](#saveZCompressed-java.lang.String-com.aspose.zip.CpioFormat-) | Arşivi Z sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveZstandard(OutputStream output)](#saveZstandard-java.io.OutputStream-) | Arşivi Zstandard sıkıştırmasıyla akışa kaydeder. |
| [saveZstandard(OutputStream output, CpioFormat cpioFormat)](#saveZstandard-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Arşivi Zstandard sıkıştırmasıyla akışa kaydeder. |
| [saveZstandard(String path)](#saveZstandard-java.lang.String-) | Arşivi Zstandard sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
| [saveZstandard(String path, CpioFormat cpioFormat)](#saveZstandard-java.lang.String-com.aspose.zip.CpioFormat-) | Arşivi Zstandard sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder. |
### CpioArchive() {#CpioArchive--}
```
public CpioArchive()
```


Yeni bir [CpioArchive](../../com.aspose.zip/cpioarchive) sınıfının örneğini başlatır.

Aşağıdaki örnek bir dosyanın nasıl sıkıştırılacağını gösterir.

```

``````

try (CpioArchive archive = new CpioArchive()) {
archive.createEntry(\"first.bin\", \"data.bin\");
archive.save(\"archive.cpio\");
}
 
```



### CpioArchive(InputStream sourceStream) {#CpioArchive-java.io.InputStream-}
```
public CpioArchive(InputStream sourceStream)
```


Initializes a new instance of the [CpioArchive](../../com.aspose.zip/cpioarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (CpioArchive archive = new CpioArchive(new FileInputStream("archive.cpio"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Bu yapıcı herhangi bir girişi açmaz. Açma işlemi için [CpioEntry.open()](../../com.aspose.zip/cpioentry\\#open--) metoduna bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceStream | java.io.InputStream | arşivin kaynağı |

### CpioArchive(String path) {#CpioArchive-java.lang.String-}
```
public CpioArchive(String path)
```


Yeni bir [CpioArchive](../../com.aspose.zip/cpioarchive) sınıfının örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

Aşağıdaki örnek, tüm girdileri bir dizine nasıl çıkarılacağını gösterir.

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [CpioEntry.open()](../../com.aspose.zip/cpioentry\#open--) method for unpacking.

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
public final CpioArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(cpioFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| directory | java.io.File | sıkıştırılacak dizin |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final CpioArchive createEntries(File directory, boolean includeRootDirectory)
```


Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler.

```

``````

try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(cpioFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final CpioArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(cpioFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceDirectory | java.lang.String | sıkıştırılacak dizin |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final CpioArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler.

```

``````

try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(cpioFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final CpioEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     java.io.File file = new File("data.bin");
     try (CpioArchive archive = new CpioArchive()) {
         archive.createEntry("test.bin", file);
         archive.save("archive.cpio");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | girişin adı |
| dosya | java.io.File | sıkıştırılacak dosya veya klasörün meta verileri |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final CpioEntry createEntry(String name, File file, boolean openImmediately)
```


Arşiv içinde tek bir giriş oluşturur.

```

``````

java.io.File file = new File("data.bin");
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("test.bin", file);
archive.save(\"archive.cpio\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final CpioEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (CpioArchive archive = new CpioArchive()) {
         archive.createEntry("data.bin", new FileInputStream("data.bin"));
         archive.save("archive.cpio");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | girişin adı |
| source | java.io.InputStream | girdi için giriş akışı |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### createEntry(String name, String sourcePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final CpioEntry createEntry(String name, String sourcePath)
```


Arşiv içinde tek bir giriş oluşturur.

```

``````

try (CpioArchive archive = new CpioArchive()) {
archive.createEntry(\"first.bin\", \"data.bin\");
archive.save(\"archive.cpio\");
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `sourcePath` parameter does not affect the entry name

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| sourcePath | java.lang.String | path to file to be compressed. |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### createEntry(String name, String sourcePath, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final CpioEntry createEntry(String name, String sourcePath, boolean openImmediately)
```


Creates a single entry within the archive.

```

``````

     try (CpioArchive archive = new CpioArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.cpio");
     }
 
```

Girdi adı yalnızca `name` parametresi içinde ayarlanır. `sourcePath` parametresinde verilen dosya adı girdi adını etkilemez.

Dosya `openImmediately` parametresiyle hemen açılırsa, arşiv serbest bırakılana kadar engellenir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | girişin adı |
| sourcePath | java.lang.String | sıkıştırılacak dosyanın yolu. |
| openImmediately | boolean | true, dosyayı hemen açmak için, aksi takdirde arşiv kaydedilirken dosyayı açar. |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### deleteEntry(CpioEntry entry) {#deleteEntry-com.aspose.zip.CpioEntry-}
```
public final CpioArchive deleteEntry(CpioEntry entry)
```


Giriş listesinden belirli bir girdinin ilk oluşumunu kaldırır.

İşte son girdiyi hariç tutarak tüm girdileri nasıl kaldırabileceğiniz:

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
while (archive.getEntries().size() > 1)
archive.deleteEntry(archive.getEntries().get(0));
archive.save("outputCpioFile.cpio");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [CpioEntry](../../com.aspose.zip/cpioentry) | the entry to remove from the entries list |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final CpioArchive deleteEntry(int entryIndex)
```


Removes the entry from the entry list by index.

```

``````

     try (CpioArchive archive = new CpioArchive("two_files.cpio")) {
         archive.deleteEntry(0);
         archive.save("single_file.cpio");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| entryIndex | int | kaldırılacak girdinin sıfır tabanlı indeksi |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - the archive with the entry deleted
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Arşivdeki tüm dosyaları verilen dizine çıkarır.

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getEntries() {#getEntries--}
```
public final List<CpioEntry> getEntries()
```


Gets entries of [CpioEntry](../../com.aspose.zip/cpioentry) type constituting the cpio archive.

**Returns:**
java.util.List&lt;com.aspose.zip.CpioEntry&gt; - entries of [CpioEntry](../../com.aspose.zip/cpioentry) type constituting the cpio archive.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the cpio archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the cpio archive.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves archive to the stream provided.

```

``````

     try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry1", "data.bin");
             archive.save(cpioFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | output | java.io.OutputStream | hedef akış. |

`output` yazılabilir olmalıdır |

### save(OutputStream output, CpioFormat cpioFormat) {#save-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void save(OutputStream output, CpioFormat cpioFormat)
```


Sağlanan akışa arşivi kaydeder.

```

``````

try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(cpioFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

```

``````

     try (CpioArchive archive = new CpioArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("archive.cpio");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | destinationFileName | java.lang.String | oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |

Bir arşivi yüklendiği aynı yola kaydetmek mümkündür. Ancak, bu yöntem geçici bir dosyaya kopyalama yaptığı için önerilmez |

### save(String destinationFileName, CpioFormat cpioFormat) {#save-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void save(String destinationFileName, CpioFormat cpioFormat)
```


Sağlanan hedef dosyaya arşivi kaydeder.

```

``````

try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(\"archive.cpio\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten.

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveGzipped(OutputStream output) {#saveGzipped-java.io.OutputStream-}
```
public final void saveGzipped(OutputStream output)
```


Saves archive to the stream with gzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.gz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveGzipped(result);
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

### saveGzipped(OutputStream output, CpioFormat cpioFormat) {#saveGzipped-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveGzipped(OutputStream output, CpioFormat cpioFormat)
```


Arşivi gzip sıkıştırmasıyla akışa kaydeder.

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.gz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped(result);
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
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveGzipped(String path) {#saveGzipped-java.lang.String-}
```
public final void saveGzipped(String path)
```


Saves archive to the file by path with gzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveGzipped("result.cpio.gz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |

### saveGzipped(String path, CpioFormat cpioFormat) {#saveGzipped-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveGzipped(String path, CpioFormat cpioFormat)
```


Arşivi gzip sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped("result.cpio.gz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveLZMACompressed(OutputStream output) {#saveLZMACompressed-java.io.OutputStream-}
```
public final void saveLZMACompressed(OutputStream output)
```


Saves the archive to the stream with LZMA compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.lzma")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZMACompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```

Önemli: cpio arşivi bu yöntemde önce oluşturulur ardından sıkıştırılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | output | java.io.OutputStream | hedef akış. |

`output` yazılabilir olmalıdır |

### saveLZMACompressed(OutputStream output, CpioFormat cpioFormat) {#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveLZMACompressed(OutputStream output, CpioFormat cpioFormat)
```


Arşivi LZMA sıkıştırmasıyla akışa kaydeder.

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.lzma")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed(result);
}
}
} catch (IOException ex) {
}
 
```

Important: cpio archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveLZMACompressed(String path) {#saveLZMACompressed-java.lang.String-}
```
public final void saveLZMACompressed(String path)
```


Saves the archive to the file by path with lzma compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZMACompressed("result.cpio.lzma");
         }
     } catch (IOException ex) {
     }
 
```

Önemli: cpio arşivi bu yöntemde önce oluşturulur ardından sıkıştırılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |

### saveLZMACompressed(String path, CpioFormat cpioFormat) {#saveLZMACompressed-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveLZMACompressed(String path, CpioFormat cpioFormat)
```


Arşivi lzma sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed("result.cpio.lzma");
}
} catch (IOException ex) {
}
 
```

Important: cpio archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveLzipped(OutputStream output) {#saveLzipped-java.io.OutputStream-}
```
public final void saveLzipped(OutputStream output)
```


Saves archive to the stream with lzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.lz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLzipped(result);
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

### saveLzipped(OutputStream output, CpioFormat cpioFormat) {#saveLzipped-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveLzipped(OutputStream output, CpioFormat cpioFormat)
```


Arşivi lzip sıkıştırmasıyla akışa kaydeder.

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.lz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
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
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveLzipped(String path) {#saveLzipped-java.lang.String-}
```
public final void saveLzipped(String path)
```


Saves archive to the file by path with lzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLzipped("result.cpio.lz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |

### saveLzipped(String path, CpioFormat cpioFormat) {#saveLzipped-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveLzipped(String path, CpioFormat cpioFormat)
```


Arşivi lzip sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped("result.cpio.lz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveXzCompressed(OutputStream output) {#saveXzCompressed-java.io.OutputStream-}
```
public final void saveXzCompressed(OutputStream output)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
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

### saveXzCompressed(OutputStream output, CpioFormat cpioFormat) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveXzCompressed(OutputStream output, CpioFormat cpioFormat)
```


Arşivi xz sıkıştırmasıyla akışa kaydeder.

```

``````

try (FileOutputStream result = new FileOutputStream(\"result.cpio.xz\")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
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
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveXzCompressed(OutputStream output, CpioFormat cpioFormat, XzArchiveSettings settings) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(OutputStream output, CpioFormat cpioFormat, XzArchiveSettings settings)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
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

`output`Akış yazılabilir olmalıdır. |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | cpio başlık formatını tanımlar |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | belirli xz arşivi ayarları kümesi: sözlük boyutu, blok boyutu, kontrol türü |

### saveXzCompressed(String path) {#saveXzCompressed-java.lang.String-}
```
public final void saveXzCompressed(String path)
```


Arşivi xz sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(\"result.cpio.xz\");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveXzCompressed(String path, CpioFormat cpioFormat) {#saveXzCompressed-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveXzCompressed(String path, CpioFormat cpioFormat)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.cpio.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | cpio başlık formatını tanımlar |

### saveXzCompressed(String path, CpioFormat cpioFormat, XzArchiveSettings settings) {#saveXzCompressed-java.lang.String-com.aspose.zip.CpioFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(String path, CpioFormat cpioFormat, XzArchiveSettings settings)
```


Arşivi xz sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(\"result.cpio.xz\");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | set of setting particular xz archive: dictionary size, block size, check type |

### saveZCompressed(OutputStream output) {#saveZCompressed-java.io.OutputStream-}
```
public final void saveZCompressed(OutputStream output)
```


Saves archive to the stream with Z compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.Z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
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
|  | output | java.io.OutputStream | hedef akış. |

`output` yazılabilir olmalıdır |

### saveZCompressed(OutputStream output, CpioFormat cpioFormat) {#saveZCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveZCompressed(OutputStream output, CpioFormat cpioFormat)
```


Arşivi Z sıkıştırmasıyla akışa kaydeder.

```

``````

try (FileOutputStream result = new FileOutputStream(\"result.cpio.Z\")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
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
| output | java.io.OutputStream | the destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveZCompressed(String path) {#saveZCompressed-java.lang.String-}
```
public final void saveZCompressed(String path)
```


Saves archive to the file by path with Z compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZCompressed("result.cpio.Z");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |

### saveZCompressed(String path, CpioFormat cpioFormat) {#saveZCompressed-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveZCompressed(String path, CpioFormat cpioFormat)
```


Arşivi Z sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed(\"result.cpio.Z\");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | d cpio header format |

### saveZstandard(OutputStream output) {#saveZstandard-java.io.OutputStream-}
```
public final void saveZstandard(OutputStream output)
```


Saves archive to the stream with Zstandard compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.zst")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
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

### saveZstandard(OutputStream output, CpioFormat cpioFormat) {#saveZstandard-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveZstandard(OutputStream output, CpioFormat cpioFormat)
```


Arşivi Zstandard sıkıştırmasıyla akışa kaydeder.

```

``````

try (FileOutputStream result = new FileOutputStream(\"result.cpio.zst\")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
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
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveZstandard(String path) {#saveZstandard-java.lang.String-}
```
public final void saveZstandard(String path)
```


Saves archive to the file by path with Zstandard compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZstandard("result.cpio.zst");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |

### saveZstandard(String path, CpioFormat cpioFormat) {#saveZstandard-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveZstandard(String path, CpioFormat cpioFormat)
```


Arşivi Zstandard sıkıştırmasıyla belirtilen yoldaki dosyaya kaydeder.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard(\"result.cpio.zst\");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

