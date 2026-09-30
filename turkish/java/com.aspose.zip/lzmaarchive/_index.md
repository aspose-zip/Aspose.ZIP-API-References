---
title: "LzmaArchive"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bu sınıf bir LZMA arşiv dosyasını temsil eder."
type: docs
weight: 86
url: /tr/java/com.aspose.zip/lzmaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzmaArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Bu sınıf LZMA arşiv dosyasını temsil eder. LZMA arşivlerini oluşturmak veya çıkarmak için kullanın.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [LzmaArchive()](#LzmaArchive--) | Yeni bir [LzmaArchive](../../com.aspose.zip/lzmaarchive) sınıfı örneği başlatır ve arşivi lzma formatında oluşturur. |
| [LzmaArchive(LzmaArchiveSettings settings)](#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-) | Yeni bir [LzmaArchive](../../com.aspose.zip/lzmaarchive) sınıfı örneği başlatır ve arşivi lzma formatında oluşturur. |
| [LzmaArchive(InputStream source)](#LzmaArchive-java.io.InputStream-) | Çıkarma için hazırlanmış yeni bir [LzmaArchive](../../com.aspose.zip/lzmaarchive) sınıfı örneği başlatır. |
| [LzmaArchive(String path)](#LzmaArchive-java.lang.String-) | Çıkarma için hazırlanmış yeni bir [LzmaArchive](../../com.aspose.zip/lzmaarchive) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | lzma arşivini bir dosyaya çıkarır. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | lzma arşivini bir akışa çıkarır. |
| [extract(String path)](#extract-java.lang.String-) | lzma arşivini yol belirterek bir dosyaya çıkarır. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Arşivin içeriğini sağlanan dizine çıkarır. |
| [getFileEntries()](#getFileEntries--) | lzma arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) tipindeki girdileri alır. |
| [getFormat()](#getFormat--) | Arşiv biçimini alır. |
| [getLength()](#getLength--) | Uzunluğu alır. |
| [getName()](#getName--) | Orijinal dosyanın adı. |
| [save(File destination)](#save-java.io.File-) | lzma arşivini sağlanan hedef dosyaya kaydeder. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | lzma arşivini sağlanan akışa kaydeder. |
| [save(String destinationFileName)](#save-java.lang.String-) | lzma arşivini sağlanan hedef dosyaya kaydeder. |
| [setSource(File file)](#setSource-java.io.File-) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
### LzmaArchive() {#LzmaArchive--}
```
public LzmaArchive()
```


Yeni bir [LzmaArchive](../../com.aspose.zip/lzmaarchive) sınıfı örneği başlatır ve arşivi lzma formatında oluşturur.

### LzmaArchive(LzmaArchiveSettings settings) {#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-}
```
public LzmaArchive(LzmaArchiveSettings settings)
```


Yeni bir [LzmaArchive](../../com.aspose.zip/lzmaarchive) sınıfı örneği başlatır ve arşivi lzma formatında oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| settings | [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) | belirli lzma arşivi ayarlarının kümesi |

### LzmaArchive(InputStream source) {#LzmaArchive-java.io.InputStream-}
```
public LzmaArchive(InputStream source)
```


Çıkarma için hazırlanmış yeni bir [LzmaArchive](../../com.aspose.zip/lzmaarchive) sınıfı örneği başlatır.

Bu yapıcı sıkıştırmayı açmaz. Sıkıştırmayı açmak için [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | java.io.InputStream | arşivin kaynağı |

### LzmaArchive(String path) {#LzmaArchive-java.lang.String-}
```
public LzmaArchive(String path)
```


Çıkarma için hazırlanmış yeni bir [LzmaArchive](../../com.aspose.zip/lzmaarchive) sınıfı örneği başlatır.

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extracts lzma archive to a file.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract(new File("extracted.bin"));
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosya | java.io.File | açılmış veriyi depolamak için dosya |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


lzma arşivini bir akışa çıkarır.

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | the stream for storing decompressed data |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts lzma archive to a file by path.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract("extracted.bin");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | açılmış verileri depolayacak dosyanın yolu |

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


lzma arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) tipindeki girdileri alır.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - lzma arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) tipindeki girdiler.
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


Uzunluğu alır.

**Returns:**
java.lang.Long - uzunluk
### getName() {#getName--}
```
public final String getName()
```


Orijinal dosyanın adı.

**Returns:**
java.lang.String - orijinal dosyanın adı
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


lzma arşivini sağlanan hedef dosyaya kaydeder.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File("data.bin"));
archive.save(new File("archive.lzma"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | the file, which will be opened as destination stream |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves lzma archive to the stream provided.

```

``````

     try (FileOutputStream lzmaFile = new FileOutputStream("archive.lzma")) {
         try (LzmaArchive archive = new LzmaArchive()) {
             archive.setSource("data.bin");
             archive.save(lzmaFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| output | java.io.OutputStream | hedef akışı |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


lzma arşivini sağlanan hedef dosyaya kaydeder.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File("data.bin"));
archive.save("result.lzma");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosya | java.io.File | dosya, giriş akışı olarak açılacak |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Arşiv içinde sıkıştırılacak içeriği ayarlar.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.lzma");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String sourcePath) {#setSource-java.lang.String-}
```
public final void setSource(String sourcePath)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourcePath | java.lang.String | dosya yolu, giriş akışı olarak açılacak |

