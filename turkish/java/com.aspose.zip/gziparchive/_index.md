---
title: "GzipArchive"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bu sınıf bir gzip arşiv dosyasını temsil eder."
type: docs
weight: 69
url: /tr/java/com.aspose.zip/gziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class GzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Bu sınıf bir gzip arşiv dosyasını temsil eder. gzip arşivlerini oluşturmak veya çıkarmak için kullanın.

Gzip sıkıştırma algoritması, LZ77 ve Huffman kodlamasının bir kombinasyonu olan DEFLATE algoritmasına dayanır.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [GzipArchive()](#GzipArchive--) | Sıkıştırma için hazırlanmış yeni bir [GzipArchive](../../com.aspose.zip/gziparchive) sınıfı örneği başlatır. |
| [GzipArchive(InputStream sourceStream)](#GzipArchive-java.io.InputStream-) | Açma için hazırlanmış yeni bir [GzipArchive](../../com.aspose.zip/gziparchive) sınıfı örneği başlatır. |
| [GzipArchive(InputStream sourceStream, boolean parseHeader)](#GzipArchive-java.io.InputStream-boolean-) | Açma için hazırlanmış yeni bir [GzipArchive](../../com.aspose.zip/gziparchive) sınıfı örneği başlatır. |
| [GzipArchive(InputStream sourceStream, GzipLoadOptions options)](#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-) | Açma için hazırlanmış yeni bir [GzipArchive](../../com.aspose.zip/gziparchive) sınıfı örneği başlatır. |
| [GzipArchive(String path, GzipLoadOptions options)](#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-) | Açma için hazırlanmış yeni bir [GzipArchive](../../com.aspose.zip/gziparchive) sınıfı örneği başlatır. |
| [GzipArchive(String path)](#GzipArchive-java.lang.String-) | Yeni bir [GzipArchive](../../com.aspose.zip/gziparchive) sınıfı örneği başlatır. |
| [GzipArchive(String path, boolean parseHeader)](#GzipArchive-java.lang.String-boolean-) | Yeni bir [GzipArchive](../../com.aspose.zip/gziparchive) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Arşivi sağlanan akıma çıkarır. |
| [extract(String path)](#extract-java.lang.String-) | Arşivi belirtilen yola dosya olarak çıkarır. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Arşivin içeriğini sağlanan dizine çıkarır. |
| [getFileEntries()](#getFileEntries--) | [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) türündeki girdileri alır ve gzip arşivini oluşturur. |
| [getFormat()](#getFormat--) | Arşiv biçimini alır. |
| [getLength()](#getLength--) | Orijinal dosyanın boyutunu alır. |
| [getName()](#getName--) | Orijinal dosyanın adı. |
| [getUncompressedSize()](#getUncompressedSize--) | Orijinal dosyanın boyutunu alır. |
| [open()](#open--) | Arşivi çıkarmak için açar ve arşiv içeriğiyle bir akış sağlar. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Sağlanan akışa arşivi kaydeder. |
| [save(String destinationFileName)](#save-java.lang.String-) | Sağlanan hedef dosyaya arşivi kaydeder. |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
| [setSource(File file)](#setSource-java.io.File-) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
| [setSource(String path)](#setSource-java.lang.String-) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
### GzipArchive() {#GzipArchive--}
```
public GzipArchive()
```


Sıkıştırma için hazırlanmış yeni bir [GzipArchive](../../com.aspose.zip/gziparchive) sınıfı örneği başlatır.

Aşağıdaki örnek bir dosyanın nasıl sıkıştırılacağını gösterir.

```

``````

try (GzipArchive archive = new GzipArchive())
{
archive.setSource(\"data.bin\");
archive.save("archive.gz");
}
 
```



### GzipArchive(InputStream sourceStream) {#GzipArchive-java.io.InputStream-}
```
public GzipArchive(InputStream sourceStream)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Bu yapıcı sıkıştırma açmaz. Açmak için [open()](../../com.aspose.zip/gziparchive\#open--) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Arşivin kaynağı. |

### GzipArchive(InputStream sourceStream, boolean parseHeader) {#GzipArchive-java.io.InputStream-boolean-}
```
public GzipArchive(InputStream sourceStream, boolean parseHeader)
```


Açma için hazırlanmış yeni bir [GzipArchive](../../com.aspose.zip/gziparchive) sınıfı örneği başlatır.

Bir akıştan arşiv aç ve `ByteArrayOutputStream`'a çıkar.

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### GzipArchive(InputStream sourceStream, GzipLoadOptions options) {#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(InputStream sourceStream, GzipLoadOptions options)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     GzipLoadOptions options = new GzipLoadOptions();
     try (GzipArchive archive = new GzipArchive(new FileInputStream("archive.gz"), options)) {
         archive.extract(ms);
     } catch (IOException ex) {
     }
 
```

Bu yapıcı sıkıştırma açmaz. Açmak için [open()](../../com.aspose.zip/gziparchive\#open--) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Arşivin kaynağı. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Arşivi yüklemek için seçenekler. |

### GzipArchive(String path, GzipLoadOptions options) {#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(String path, GzipLoadOptions options)
```


Açma için hazırlanmış yeni bir [GzipArchive](../../com.aspose.zip/gziparchive) sınıfı örneği başlatır.

Dosyadan yolu kullanarak bir arşiv aç ve onu bir `MemoryStream`'e çıkar.

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
GzipLoadOptions options = new GzipLoadOptions();
try (GzipArchive archive = new GzipArchive("archive.gz", options)) {
archive.extract(ms);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Options to load the archive with. |

### GzipArchive(String path) {#GzipArchive-java.lang.String-}
```
public GzipArchive(String path)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Bu yapıcı sıkıştırma açmaz. Açmak için [open()](../../com.aspose.zip/gziparchive\#open--) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | Arşiv dosyasının yolu. |

### GzipArchive(String path, boolean parseHeader) {#GzipArchive-java.lang.String-boolean-}
```
public GzipArchive(String path, boolean parseHeader)
```


Yeni bir [GzipArchive](../../com.aspose.zip/gziparchive) sınıfı örneği başlatır.

Dosyadan yolu kullanarak bir arşiv aç ve onu bir `MemoryStream`'e çıkar.

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive("archive.gz")) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

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

     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hedef | java.io.OutputStream | Hedef akış. Yazılabilir olmalıdır. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Arşivi belirtilen yola dosya olarak çıkarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | Hedef dosyanın yolu. Dosya zaten mevcutsa, üzerine yazılacaktır. |

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
|  | destinationDirectory | java.lang.String | Çıkarılan dosyaların yerleştirileceği dizinin yolu. |

Dizin mevcut değilse, oluşturulacaktır. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


[IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) türündeki girdileri alır ve gzip arşivini oluşturur.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - gzip arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) tipindeki girişler.
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


Orijinal dosyanın boyutunu alır.

Sıkıştırma açma sırasında, bu özellik yanlış boyut içerebilir. Açılmış dosya boyutu 4 GB'yi aşarsa, başlıktaki 32‑bit sınırlama nedeniyle bu özellik hatalı bir değer verir.

**Returns:**
java.lang.Long - orijinal dosyanın boyutu
### getName() {#getName--}
```
public final String getName()
```


Orijinal dosyanın adı.

**Returns:**
java.lang.String - orijinal dosyanın adı
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Orijinal dosyanın boyutunu alır.

Sıkıştırma açma sırasında, bu özellik yanlış boyut içerebilir. Açılmış dosya boyutu 4 GB'yi aşarsa, başlıktaki 32‑bit sınırlama nedeniyle bu özellik hatalı bir değer verir.

**Returns:**
long - orijinal dosyanın boyutu.
### open() {#open--}
```
public final InputStream open()
```


Arşivi çıkarmak için açar ve arşiv içeriğiyle bir akış sağlar.

Arşivi çıkarır ve çıkarılan içeriği dosya akışına kopyalar.

```

``````

try (GzipArchive archive = new GzipArchive("archive.gz")) {
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

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - The stream that represents the contents of the archive.
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Writes compressed data to http response stream.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(httpResponseStream);
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | outputStream | java.io.OutputStream | Hedef akış. |

`outputStream` yazılabilir olmalıdır. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Sağlanan hedef dosyaya arşivi kaydeder.

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource(\"data.bin\");
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### setSource(TarArchive tarArchive) {#setSource-com.aspose.zip.TarArchive-}
```
public final void setSource(TarArchive tarArchive)
```


Sets the content to be compressed within the archive.

```

``````

     try (TarArchive tarArchive = new TarArchive()) {
         tarArchive.createEntry("first.bin", "data1.bin");
         tarArchive.createEntry("second.bin", "data2.bin");
         try (GzipArchive gzippedArchive = new GzipArchive()) {
             gzippedArchive.setSource(tarArchive);
             gzippedArchive.save("archive.tar.gz");
         }
     }
 
```

Bu yöntemi ortak bir tar.gz arşivi oluşturmak için kullanın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | Sıkıştırılacak Tar arşivi. |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Arşiv içinde sıkıştırılacak içeriği ayarlar.

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource(new File("data.bin"));
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | The reference to a file to be compressed. |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.gz");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | java.io.InputStream | Arşiv için giriş akışı. |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Arşiv içinde sıkıştırılacak içeriği ayarlar.

Dosyadan yolu kullanarak bir arşiv aç ve onu bir `MemoryStream`'e çıkar.

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource(\"data.bin\");
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file to be compressed. |

