---
title: "IsoArchive"
second_title: "Aspose.ZIP for Java API Referansı"
description: "ISO 9660 ISO arşivini temsil eder."
type: docs
weight: 71
url: /tr/java/com.aspose.zip/isoarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public final class IsoArchive implements IArchive, AutoCloseable
```

Bir ISO arşivi (ISO 9660) temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [IsoArchive()](#IsoArchive--) | Yeni bir [IsoArchive](../../com.aspose.zip/isoarchive) sınıfının örneğini başlatır ve yeni dosya ve dizinler eklemek için boş bir ISO arşivi oluşturur. |
| [IsoArchive(InputStream sourceStream)](#IsoArchive-java.io.InputStream-) | Yeni bir [IsoArchive](../../com.aspose.zip/isoarchive) sınıfının örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)](#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-) | Yeni bir [IsoArchive](../../com.aspose.zip/isoarchive) sınıfının örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [IsoArchive(String path)](#IsoArchive-java.lang.String-) | Yeni bir [IsoArchive](../../com.aspose.zip/isoarchive) sınıfının örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| [IsoArchive(String path, IsoLoadOptions loadOptions)](#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-) | Yeni bir [IsoArchive](../../com.aspose.zip/isoarchive) sınıfının örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createDirectory(String name)](#createDirectory-java.lang.String-) | ISO görüntüsüne bir dizin ekler. |
| [createEntry(String name)](#createEntry-java.lang.String-) | ISO görüntüsüne bir dosya ekler. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | ISO görüntüsüne bir dosya ekler. |
| [createEntry(String name, String filePath)](#createEntry-java.lang.String-java.lang.String-) | ISO görüntüsüne bir dosya ekler. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Tüm girişleri belirtilen dizine çıkarır. |
| [getEntries()](#getEntries--) | Arşivi oluşturan [IsoEntry](../../com.aspose.zip/isoentry) türündeki girişleri alır. |
| [getFileEntries()](#getFileEntries--) | Arşivi oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) türündeki girişleri alır. |
| [getFormat()](#getFormat--) | Arşiv biçimini alır. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | ISO görüntüsünü belirtilen akışa kaydeder. |
| [save(OutputStream stream, IsoSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-) | ISO görüntüsünü belirtilen akışa kaydeder. |
| [save(String path)](#save-java.lang.String-) | ISO görüntüsünü belirtilen yola kaydeder. |
| [save(String path, IsoSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.IsoSaveOptions-) | ISO görüntüsünü belirtilen yola kaydeder. |
### IsoArchive() {#IsoArchive--}
```
public IsoArchive()
```


Yeni bir [IsoArchive](../../com.aspose.zip/isoarchive) sınıfının örneğini başlatır ve yeni dosya ve dizinler eklemek için boş bir ISO arşivi oluşturur.

Aşağıdaki örnek, yeni boş bir ISO arşivi oluşturmayı ve dosyaları eklemeyi gösterir:

```

``````

// Yeni boş bir ISO arşivi oluştur
try (IsoArchive isoArchive = new IsoArchive()) {
// ISO arşivine dosyalar ekle
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// ISO arşivini bir dosyaya kaydet
isoArchive.save("new_archive.iso");
}
 
```



### IsoArchive(InputStream sourceStream) {#IsoArchive-java.io.InputStream-}
```
public IsoArchive(InputStream sourceStream)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Bu yapıcı, herhangi bir girdiyi açmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceStream | java.io.InputStream | arşivin kaynağı |

### IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions) {#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)
```


Yeni bir [IsoArchive](../../com.aspose.zip/isoarchive) sınıfının örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

Aşağıdaki örnek, tüm girdileri bir dizine nasıl çıkarılacağını gösterir.

```

``````

try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### IsoArchive(String path) {#IsoArchive-java.lang.String-}
```
public IsoArchive(String path)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive("archive.iso")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

Bu yapıcı, herhangi bir girdiyi açmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | arşiv dosyasının yolu |

### IsoArchive(String path, IsoLoadOptions loadOptions) {#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(String path, IsoLoadOptions loadOptions)
```


Yeni bir [IsoArchive](../../com.aspose.zip/isoarchive) sınıfının örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur.

Aşağıdaki örnek, tüm girdileri bir dizine nasıl çıkarılacağını gösterir.

```

``````

try (IsoArchive archive = new IsoArchive("archive.iso")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### close() {#close--}
```
public void close()
```




### createDirectory(String name) {#createDirectory-java.lang.String-}
```
public final IsoEntry createDirectory(String name)
```


Adds a directory to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the directory in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name) {#createEntry-java.lang.String-}
```
public final IsoEntry createEntry(String name)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final IsoEntry createEntry(String name, InputStream source)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| source | java.io.InputStream | the stream containing the file data |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, String filePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final IsoEntry createEntry(String name, String filePath)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| filePath | java.lang.String | the path of the file |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all entries to the specified directory.

The following example shows how to extract all entries to a directory:

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationDirectory | java.lang.String | girdilerin çıkarılacağı dizin |

### getEntries() {#getEntries--}
```
public final List<IsoEntry> getEntries()
```


Arşivi oluşturan [IsoEntry](../../com.aspose.zip/isoentry) türündeki girişleri alır.

**Returns:**
java.util.List&lt;com.aspose.zip.IsoEntry&gt; - ISO arşivini oluşturan [IsoEntry](../../com.aspose.zip/isoentry) tipindeki girdiler
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Arşivi oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) türündeki girişleri alır.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - ISO arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) tipindeki girdiler
### getFormat() {#getFormat--}
```
public ArchiveFormat getFormat()
```


Arşiv biçimini alır.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream stream)
```


ISO görüntüsünü belirtilen akışa kaydeder.

Aşağıdaki örnek, bir ISO arşivini bellek akışına nasıl kaydedeceğinizi gösterir:

```

``````

ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
// Yeni boş bir ISO arşivi oluştur
try (IsoArchive isoArchive = new IsoArchive()) {
// ISO arşivine dosyalar ekle
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// ISO arşivini bellek akışına kaydet
isoArchive.save(memoryStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the stream where the ISO image will be saved |

### save(OutputStream stream, IsoSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-}
```
public final void save(OutputStream stream, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified stream.

The following example shows how to save an ISO archive to a memory stream:

```

``````

     ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a memory stream
         isoArchive.save(memoryStream);
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.OutputStream | ISO görüntüsünün kaydedileceği akış |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | ISO arşivini kaydetmek için seçenekler |

### save(String path) {#save-java.lang.String-}
```
public final void save(String path)
```


ISO görüntüsünü belirtilen yola kaydeder.

Aşağıdaki örnek, bir ISO arşivinin bir dosyaya nasıl kaydedileceğini gösterir:

```

``````

// Yeni boş bir ISO arşivi oluştur
try (IsoArchive isoArchive = new IsoArchive()) {
// ISO arşivine dosyalar ekle
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// ISO arşivini bir dosyaya kaydet
isoArchive.save("new_archive.iso");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path where the ISO image will be saved |

### save(String path, IsoSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.IsoSaveOptions-}
```
public final void save(String path, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified path.

The following example shows how to save an ISO archive to a file:

```

``````

     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a file
         isoArchive.save("new_archive.iso");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | ISO görüntüsünün kaydedileceği yol |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | ISO arşivini kaydetmek için seçenekler |

