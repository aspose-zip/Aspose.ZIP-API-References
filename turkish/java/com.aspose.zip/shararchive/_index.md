---
title: "SharArchive"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bu sınıf bir shar arşiv dosyasını temsil eder."
type: docs
weight: 119
url: /tr/java/com.aspose.zip/shararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class SharArchive implements AutoCloseable
```

Bu sınıf bir shar arşiv dosyasını temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SharArchive()](#SharArchive--) | Yeni bir [SharArchive](../../com.aspose.zip/shararchive) sınıfının örneğini başlatır. |
| [SharArchive(String path)](#SharArchive-java.lang.String-) | Ayrıştırma için hazırlanmış yeni bir [SharArchive](../../com.aspose.zip/shararchive) sınıfının örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Arşiv içinde tek bir giriş oluşturur. |
| [createEntry(String name, File file, boolean includeRootDirectory)](#createEntry-java.lang.String-java.io.File-boolean-) | Arşiv içinde tek bir giriş oluştur. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Arşiv içinde tek bir giriş oluştur. |
| [createEntry(String name, String sourcePath)](#createEntry-java.lang.String-java.lang.String-) | Arşiv içinde tek bir giriş oluştur. |
| [createEntry(String name, String sourcePath, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Arşiv içinde tek bir giriş oluştur. |
| [deleteEntry(SharEntry entry)](#deleteEntry-com.aspose.zip.SharEntry-) | Giriş listesinden belirli bir girdinin ilk oluşumunu kaldırır. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Giriş listesinden girdiyi indeksine göre kaldırır. |
| [getEntries()](#getEntries--) | Arşivi oluşturan [SharEntry](../../com.aspose.zip/sharentry) türündeki girdileri alır. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Sağlanan akışa arşivi kaydeder. |
| [save(String destinationFileName)](#save-java.lang.String-) | Sağlanan hedef dosyaya arşivi kaydeder. |
### SharArchive() {#SharArchive--}
```
public SharArchive()
```


Yeni bir [SharArchive](../../com.aspose.zip/shararchive) sınıfının örneğini başlatır.

Aşağıdaki örnek bir dosyanın nasıl sıkıştırılacağını gösterir.

```

``````

try (SharArchive archive = new SharArchive()) {
archive.createEntry(\"first.bin\", \"data.bin\");
archive.save("archive.shar");
}
 
```



### SharArchive(String path) {#SharArchive-java.lang.String-}
```
public SharArchive(String path)
```


Initializes a new instance of the [SharArchive](../../com.aspose.zip/shararchive) class prepared for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final SharArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
         try (SharArchive archive = new SharArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(sharFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| directory | java.io.File | sıkıştırılacak dizin |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final SharArchive createEntries(File directory, boolean includeRootDirectory)
```


Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler.

```

``````

try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
try (SharArchive archive = new SharArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(sharFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | the directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final SharArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
         try (SharArchive archive = new SharArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(sharFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceDirectory | java.lang.String | sıkıştırılacak dizin |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final SharArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler.

```

``````

try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
try (SharArchive archive = new SharArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(sharFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | the directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final SharEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     java.io.File file = new java.io.File("data.bin");
     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("test.bin", file);
         archive.save("archive.shar");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | girişin adı |
| dosya | java.io.File | sıkıştırılacak dosya veya klasörün meta verileri |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, File file, boolean includeRootDirectory) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final SharEntry createEntry(String name, File file, boolean includeRootDirectory)
```


Arşiv içinde tek bir giriş oluştur.

```

``````

java.io.File file = new java.io.File("data.bin");
try (SharArchive archive = new SharArchive()) {
archive.createEntry("test.bin", file);
archive.save("archive.shar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final SharEntry createEntry(String name, InputStream source)
```


Create a single entry within the archive.

```

``````

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("data.bin", new FileInputStream("data.bin"));
         archive.save("archive.shar");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | girişin adı |
| source | java.io.InputStream | girdi için giriş akışı |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, String sourcePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final SharEntry createEntry(String name, String sourcePath)
```


Arşiv içinde tek bir giriş oluştur.

```

``````

try (SharArchive archive = new SharArchive()) {
archive.createEntry(\"first.bin\", \"data.bin\");
archive.save("archive.shar");
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `sourcePath` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| sourcePath | java.lang.String | the path to the file to be compressed |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final SharEntry createEntry(String name, String sourcePath, boolean openImmediately)
```


Create a single entry within the archive.

```

``````

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.shar");
     }
 
```

Giriş adı yalnızca `name` parametresi içinde ayarlanır. `sourcePath` parametresinde verilen dosya adı giriş adını etkilemez.

`openImmediately` parametresiyle dosya hemen açılırsa, arşiv serbest bırakılana kadar dosya engellenir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | girişin adı |
| sourcePath | java.lang.String | sıkıştırılacak dosyanın yolu |
| openImmediately | boolean | doğru, dosyayı hemen açmak için, aksi takdirde arşiv kaydedilirken dosyayı açar |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### deleteEntry(SharEntry entry) {#deleteEntry-com.aspose.zip.SharEntry-}
```
public final SharArchive deleteEntry(SharEntry entry)
```


Giriş listesinden belirli bir girdinin ilk oluşumunu kaldırır.

İşte son girdiyi hariç tutarak tüm girdileri nasıl kaldırabileceğiniz:

```

``````

try (SharArchive archive = new SharArchive("archive.shar")) {
while (archive.getEntries().size() > 1)
archive.deleteEntry(archive.getEntries().get(0));
archive.save("outputSharFile.shar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [SharEntry](../../com.aspose.zip/sharentry) | the entry to remove from the entries list |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final SharArchive deleteEntry(int entryIndex)
```


Removes the entry from the entry list by index.

```

``````

     try (SharArchive archive = new SharArchive("two_files.shar")) {
         archive.deleteEntry(0);
         archive.save("single_file.shar");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| entryIndex | int | kaldırılacak girdinin sıfır tabanlı indeksi |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - the archive with the entry deleted
### getEntries() {#getEntries--}
```
public final List<SharEntry> getEntries()
```


Arşivi oluşturan [SharEntry](../../com.aspose.zip/sharentry) türündeki girdileri alır.

**Returns:**
java.util.List&lt;com.aspose.zip.SharEntry&gt; - arşivi oluşturan [SharEntry](../../com.aspose.zip/sharentry) türündeki girdiler
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Sağlanan akışa arşivi kaydeder.

```

``````

try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
try (SharArchive archive = new SharArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(sharFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

```

``````

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("archive.shar");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | destinationFileName | java.lang.String | oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |

Bir arşivi yüklendiği aynı yola kaydetmek mümkündür. Ancak, bu yöntem geçici bir dosyaya kopyalama yaptığı için önerilmez |

