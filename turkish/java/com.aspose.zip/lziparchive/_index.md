---
title: "LzipArchive"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bu sınıf bir Lzip arşiv dosyasını temsil eder."
type: docs
weight: 83
url: /tr/java/com.aspose.zip/lziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Bu sınıf bir Lzip arşiv dosyasını temsil eder. Lzip arşivlerini oluşturmak veya çıkarmak için kullanın.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [LzipArchive()](#LzipArchive--) | Yeni bir [LzipArchive](../../com.aspose.zip/lziparchive) örneği başlatır. |
| [LzipArchive(LzipArchiveSettings settings)](#LzipArchive-com.aspose.zip.LzipArchiveSettings-) | Yeni bir [LzipArchive](../../com.aspose.zip/lziparchive) örneği başlatır. |
| [LzipArchive(InputStream sourceStream)](#LzipArchive-java.io.InputStream-) | Çıkarma işlemi için hazırlanmış [LzipArchive](../../com.aspose.zip/lziparchive) sınıfının yeni bir örneğini başlatır. |
| [LzipArchive(InputStream sourceStream, LzipLoadOptions options)](#LzipArchive-java.io.InputStream-com.aspose.zip.LzipLoadOptions-) | Çıkarma işlemi için hazırlanmış [LzipArchive](../../com.aspose.zip/lziparchive) sınıfının yeni bir örneğini başlatır. |
| [LzipArchive(String path)](#LzipArchive-java.lang.String-) | Çıkarma işlemi için hazırlanmış [LzipArchive](../../com.aspose.zip/lziparchive) sınıfının yeni bir örneğini başlatır. |
| [LzipArchive(String path, LzipLoadOptions options)](#LzipArchive-java.lang.String-com.aspose.zip.LzipLoadOptions-) | Çıkarma işlemi için hazırlanmış [LzipArchive](../../com.aspose.zip/lziparchive) sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Lzip arşivini bir dosyaya çıkarır. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Lzip arşivini bir akışa çıkarır. |
| [extract(String path)](#extract-java.lang.String-) | Lzip arşivini yol belirterek bir dosyaya çıkarır. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Arşivin içeriğini sağlanan dizine çıkarır. |
| [getFileEntries()](#getFileEntries--) | Lzip arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) tipindeki girdileri alır. |
| [getFormat()](#getFormat--) | Arşiv biçimini alır. |
| [getLength()](#getLength--) | Uzunluğu alır. |
| [getName()](#getName--) | Orijinal dosyanın adı. |
| [getSettings()](#getSettings--) | Belirli bir lzip arşivinin ayarını alır. |
| [getUncompressedSize()](#getUncompressedSize--) | Dosya verisinin sıkıştırılmamış boyutunu bayt cinsinden alır. |
| [save(File destination)](#save-java.io.File-) | Lzip arşivini sağlanan hedef dosyaya kaydeder. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Lzip arşivini sağlanan akışa kaydeder. |
| [save(String destinationFileName)](#save-java.lang.String-) | Lzip arşivini sağlanan hedef dosyaya kaydeder. |
| [setSource(File file)](#setSource-java.io.File-) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
| [setSource(String path)](#setSource-java.lang.String-) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
### LzipArchive() {#LzipArchive--}
```
public LzipArchive()
```


Yeni bir [LzipArchive](../../com.aspose.zip/lziparchive) örneği başlatır.

### LzipArchive(LzipArchiveSettings settings) {#LzipArchive-com.aspose.zip.LzipArchiveSettings-}
```
public LzipArchive(LzipArchiveSettings settings)
```


Yeni bir [LzipArchive](../../com.aspose.zip/lziparchive) örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| settings | [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) | Sözlük boyutu tanımıyla belirli bir lzip arşivinin ayarı |

### LzipArchive(InputStream sourceStream) {#LzipArchive-java.io.InputStream-}
```
public LzipArchive(InputStream sourceStream)
```


Çıkarma işlemi için hazırlanmış [LzipArchive](../../com.aspose.zip/lziparchive) sınıfının yeni bir örneğini başlatır.

```

``````

try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### LzipArchive(InputStream sourceStream, LzipLoadOptions options) {#LzipArchive-java.io.InputStream-com.aspose.zip.LzipLoadOptions-}
```
public LzipArchive(InputStream sourceStream, LzipLoadOptions options)
```


Initializes a new instance of the [LzipArchive](../../com.aspose.zip/lziparchive) class prepared for decompressing.

```

``````

     try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```

Bu yapıcı sıkıştırma açmaz. Sıkıştırma açmak için [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceStream | java.io.InputStream | arşivin kaynağı |
| options | [LzipLoadOptions](../../com.aspose.zip/lziploadoptions) | Arşivi yüklemek için seçenekler. |

### LzipArchive(String path) {#LzipArchive-java.lang.String-}
```
public LzipArchive(String path)
```


Çıkarma işlemi için hazırlanmış [LzipArchive](../../com.aspose.zip/lziparchive) sınıfının yeni bir örneğini başlatır.

```

``````

try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
try (LzipArchive archive = new LzipArchive("sourceLzipFileName")) {
archive.extract(extractedFile);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### LzipArchive(String path, LzipLoadOptions options) {#LzipArchive-java.lang.String-com.aspose.zip.LzipLoadOptions-}
```
public LzipArchive(String path, LzipLoadOptions options)
```


Initializes a new instance of the [LzipArchive](../../com.aspose.zip/lziparchive) class prepared for decompressing.

```

``````

     try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
         try (LzipArchive archive = new LzipArchive("sourceLzipFileName")) {
             archive.extract(extractedFile);
         }
     } catch (IOException ex) {
     }
 
```

Bu yapıcı sıkıştırma açmaz. Sıkıştırma açmak için [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | arşivin kaynağına giden yol |
| options | [LzipLoadOptions](../../com.aspose.zip/lziploadoptions) | Arşivi yüklemek için seçenekler. |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Lzip arşivini bir dosyaya çıkarır.

```

``````

try (FileInputStream lzipFile = new FileInputStream("sourceFileName")) {
try (LzipArchive archive = new LzipArchive(lzipFile)) {
archive.extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts lzip archive to a stream.

```

``````

     try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hedef | java.io.OutputStream | açılmış veriyi depolamak için akış |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Lzip arşivini yol belirterek bir dosyaya çıkarır.

```

``````

try (FileInputStream lzipFile = new FileInputStream("sourceFileName")) {
try (LzipArchive archive = new LzipArchive(lzipFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file which will store decompressed data |

**Returns:**
java.io.File - the file info of the extracted file
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the lzip archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the lzip archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length
### getName() {#getName--}
```
public final String getName()
```


The name of original file.

**Returns:**
java.lang.String - the name of the original file
### getSettings() {#getSettings--}
```
public final LzipArchiveSettings getSettings()
```


Gets the setting of particular lzip archive.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the setting of particular lzip archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the file data in bytes.

**Returns:**
long - the uncompressed size of the file data in bytes
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves lzip archive to destination file provided.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.lz"));
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hedef | java.io.File | dosya, hedef akış olarak açılacak |

### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Lzip arşivini sağlanan akışa kaydeder.

```

``````

try (FileOutputStream lzFile = new FileOutputStream("archive.lz")) {
try (LzipArchive archive = new LzipArchive()) {
archive.setSource(\"data.bin\");
archive.save(lzFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves lzip archive to destination file provided.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.lz");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationFileName | java.lang.String | oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Arşiv içinde sıkıştırılacak içeriği ayarlar.

```

``````

try (LzipArchive archive = new LzipArchive()) {
archive.setSource(new File("data.bin"));
archive.save("archive.lz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file which will be opened as input stream |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF} ));
         archive.save("archive.lz");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | java.io.InputStream | arşiv için giriş akışı |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Arşiv içinde sıkıştırılacak içeriği ayarlar.

```

``````

try (LzipArchive archive = new LzipArchive()) {
archive.setSource(\"data.bin\");
archive.save("archive.lz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file to be compressed |

