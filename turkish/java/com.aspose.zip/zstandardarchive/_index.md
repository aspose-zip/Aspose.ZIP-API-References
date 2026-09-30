---
title: "ZstandardArchive"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bu sınıf bir Zstandard arşiv dosyasını temsil eder."
type: docs
weight: 156
url: /tr/java/com.aspose.zip/zstandardarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ZstandardArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

Bu sınıf bir Zstandard arşiv dosyasını temsil eder. Zstandard arşivleri oluşturmak için kullanın.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ZstandardArchive()](#ZstandardArchive--) | Sıkıştırma için hazırlanmış [ZstandardArchive](../../com.aspose.zip/zstandardarchive) sınıfının yeni bir örneğini başlatır. |
| [ZstandardArchive(InputStream sourceStream)](#ZstandardArchive-java.io.InputStream-) | Sıkıştırmayı açma için hazırlanmış [ZstandardArchive](../../com.aspose.zip/zstandardarchive) sınıfının yeni bir örneğini başlatır. |
| [ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options)](#ZstandardArchive-java.io.InputStream-com.aspose.zip.ZstandardLoadOptions-) | Sıkıştırmayı açma için hazırlanmış [ZstandardArchive](../../com.aspose.zip/zstandardarchive) sınıfının yeni bir örneğini başlatır. |
| [ZstandardArchive(String path)](#ZstandardArchive-java.lang.String-) | [ZstandardArchive](../../com.aspose.zip/zstandardarchive) sınıfının yeni bir örneğini başlatır. |
| [ZstandardArchive(String path, ZstandardLoadOptions options)](#ZstandardArchive-java.lang.String-com.aspose.zip.ZstandardLoadOptions-) | [ZstandardArchive](../../com.aspose.zip/zstandardarchive) sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Arşivi sağlanan akıma çıkarır. |
| [extract(String path)](#extract-java.lang.String-) | Arşivi belirtilen yola dosya olarak çıkarır. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Arşivin içeriğini sağlanan dizine çıkarır. |
| [getFileEntries()](#getFileEntries--) | zstandard arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) tipindeki girişleri alır. |
| [getFormat()](#getFormat--) | Arşiv biçimini alır. |
| [getLength()](#getLength--) | Girdinin uzunluğunu bayt cinsinden alır. |
| [getName()](#getName--) | Arşiv içindeki girişin adını alır. |
| [open()](#open--) | Arşivi çıkarmak için açar ve arşiv içeriğiyle bir akış sağlar. |
| [save(File destination)](#save-java.io.File-) | Sağlanan hedef dosyaya arşivi kaydeder. |
| [save(File destination, ZstandardSaveOptions settings)](#save-java.io.File-com.aspose.zip.ZstandardSaveOptions-) | Sağlanan hedef dosyaya arşivi kaydeder. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Sağlanan akışa arşivi kaydeder. |
| [save(OutputStream outputStream, ZstandardSaveOptions settings)](#save-java.io.OutputStream-com.aspose.zip.ZstandardSaveOptions-) | Sağlanan akışa arşivi kaydeder. |
| [save(String destinationFileName)](#save-java.lang.String-) | Sağlanan hedef dosyaya arşivi kaydeder. |
| [save(String destinationFileName, ZstandardSaveOptions settings)](#save-java.lang.String-com.aspose.zip.ZstandardSaveOptions-) | Sağlanan hedef dosyaya arşivi kaydeder. |
| [setSource(File file)](#setSource-java.io.File-) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
| [setSource(String path)](#setSource-java.lang.String-) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
### ZstandardArchive() {#ZstandardArchive--}
```
public ZstandardArchive()
```


Sıkıştırma için hazırlanmış [ZstandardArchive](../../com.aspose.zip/zstandardarchive) sınıfının yeni bir örneğini başlatır.

Aşağıdaki örnek bir dosyanın nasıl sıkıştırılacağını gösterir.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(\"data.bin\");
archive.save("archive.zst");
}
 
```



### ZstandardArchive(InputStream sourceStream) {#ZstandardArchive-java.io.InputStream-}
```
public ZstandardArchive(InputStream sourceStream)
```


Initializes a new instance of the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (ZstandardArchive archive = new ZstandardArchive(new FileInputStream("archive.zst"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Bu yapıcı sıkıştırmayı açmaz. Sıkıştırmayı açmak için [open()](../../com.aspose.zip/zstandardarchive\\#open--) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceStream | java.io.InputStream | arşivin kaynağı |

### ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options) {#ZstandardArchive-java.io.InputStream-com.aspose.zip.ZstandardLoadOptions-}
```
public ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options)
```


Sıkıştırmayı açma için hazırlanmış [ZstandardArchive](../../com.aspose.zip/zstandardarchive) sınıfının yeni bir örneğini başlatır.

Bir akıştan arşiv aç ve `ByteArrayOutputStream`'a çıkar.

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (ZstandardArchive archive = new ZstandardArchive(new FileInputStream("archive.zst"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/zstandardarchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| options | [ZstandardLoadOptions](../../com.aspose.zip/zstandardloadoptions) | the options to load archive with |

### ZstandardArchive(String path) {#ZstandardArchive-java.lang.String-}
```
public ZstandardArchive(String path)
```


Initializes a new instance of the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) class.

Open an archive from file by path and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Bu yapıcı sıkıştırmayı açmaz. Sıkıştırmayı açmak için [open()](../../com.aspose.zip/zstandardarchive\\#open--) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | arşiv dosyasının yolu |

### ZstandardArchive(String path, ZstandardLoadOptions options) {#ZstandardArchive-java.lang.String-com.aspose.zip.ZstandardLoadOptions-}
```
public ZstandardArchive(String path, ZstandardLoadOptions options)
```


[ZstandardArchive](../../com.aspose.zip/zstandardarchive) sınıfının yeni bir örneğini başlatır.

Dosya yolundan bir arşiv aç ve `ByteArrayOutputStream`'a çıkar.

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/zstandardarchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| options | [ZstandardLoadOptions](../../com.aspose.zip/zstandardloadoptions) | the options to load archive with |

### close() {#close--}
```
public void close()
```




### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the archive to the stream provided.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hedef | java.io.OutputStream | hedef akış. Yazılabilir olmalıdır |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Arşivi belirtilen yola dosya olarak çıkarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | hedef dosyanın yolu. Dosya zaten mevcutsa, üzerine yazılacaktır. |

**Returns:**
java.io.File - çıkarılan dosyanın dosya bilgisi
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Arşivin içeriğini sağlanan dizine çıkarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | çıkarılan dosyaların yerleştirileceği dizine giden yol. |

Dizin mevcut değilse, oluşturulacaktır |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


zstandard arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) tipindeki girişleri alır.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - zstandard arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) tipindeki girişler
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Arşiv biçimini alır.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


Girdinin uzunluğunu bayt cinsinden alır.

**Returns:**
java.lang.Long - girişin bayt cinsinden uzunluğu
### getName() {#getName--}
```
public final String getName()
```


Arşiv içindeki girişin adını alır.

**Returns:**
java.lang.String - arşiv içindeki girişin adı
### open() {#open--}
```
public final InputStream open()
```


Arşivi çıkarmak için açar ve arşiv içeriğiyle bir akış sağlar.

Arşivi çıkarır ve çıkarılan içeriği dosya akışına kopyalar.

```

``````

try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
try (FileOutputStream extracted = new FileOutputStream("data.bin")) {
InputStream unpacked = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the archive
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves archive to the destination file provided.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.zst"));
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hedef | java.io.File | hedef akış olarak açılacak dosya |

### save(File destination, ZstandardSaveOptions settings) {#save-java.io.File-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(File destination, ZstandardSaveOptions settings)
```


Sağlanan hedef dosyaya arşivi kaydeder.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new File("data.bin"));
archive.save(new File("archive.zst"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | the file, which will be opened as destination stream |
| settings | [ZstandardSaveOptions](../../com.aspose.zip/zstandardsaveoptions) | the settings for archive composition |

### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Write compressed data to http response stream.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(outputStream);
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| outputStream | java.io.OutputStream | hedef akış |

### save(OutputStream outputStream, ZstandardSaveOptions settings) {#save-java.io.OutputStream-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(OutputStream outputStream, ZstandardSaveOptions settings)
```


Sağlanan akışa arşivi kaydeder.

Sıkıştırılmış veriyi http yanıt akışına yazın.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new File("data.bin"));
archive.save(outputStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | the destination stream |
| settings | [ZstandardSaveOptions](../../com.aspose.zip/zstandardsaveoptions) | the settings for archive composition |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.zst");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationFileName | java.lang.String | oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |

### save(String destinationFileName, ZstandardSaveOptions settings) {#save-java.lang.String-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(String destinationFileName, ZstandardSaveOptions settings)
```


Sağlanan hedef dosyaya arşivi kaydeder.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new File("data.bin"));
archive.save("result.zst");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| settings | [ZstandardSaveOptions](../../com.aspose.zip/zstandardsaveoptions) | the settings for archive composition |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.zst");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosya | java.io.File | sıkıştırılacak dosyaya referans |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Arşiv içinde sıkıştırılacak içeriği ayarlar.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save("archive.zst");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.zst");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | sıkıştırılacak dosyanın yolu |

