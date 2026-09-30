---
title: "XzArchive"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bu sınıf xz arşiv dosyasını temsil eder."
type: docs
weight: 146
url: /tr/java/com.aspose.zip/xzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class XzArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

Bu sınıf xz arşiv dosyasını temsil eder. xz arşivlerini oluşturmak ve çıkarmak için kullanın.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [XzArchive()](#XzArchive--) | Yeni bir [XzArchive](../../com.aspose.zip/xzarchive) sınıfı örneği başlatır ve arşivi xz formatında oluşturur. |
| [XzArchive(XzArchiveSettings settings)](#XzArchive-com.aspose.zip.XzArchiveSettings-) | Yeni bir [XzArchive](../../com.aspose.zip/xzarchive) sınıfı örneği başlatır ve arşivi xz formatında oluşturur. |
| [XzArchive(InputStream source)](#XzArchive-java.io.InputStream-) | Yeni bir [XzArchive](../../com.aspose.zip/xzarchive) sınıfı örneği başlatır ve açma işlemi için hazırlar. |
| [XzArchive(InputStream source, XzLoadOptions options)](#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-) | Yeni bir [XzArchive](../../com.aspose.zip/xzarchive) sınıfı örneği başlatır ve açma işlemi için hazırlar. |
| [XzArchive(String path)](#XzArchive-java.lang.String-) | Yeni bir [XzArchive](../../com.aspose.zip/xzarchive) sınıfı örneği başlatır ve açma işlemi için hazırlar. |
| [XzArchive(String path, XzLoadOptions options)](#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-) | Yeni bir [XzArchive](../../com.aspose.zip/xzarchive) sınıfı örneği başlatır ve açma işlemi için hazırlar. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | xz arşivini bir dosyaya çıkarır. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | xz arşivini bir akışa çıkarır. |
| [extract(String path)](#extract-java.lang.String-) | xz arşivini yol belirterek bir dosyaya çıkarır. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Arşivin içeriğini sağlanan dizine çıkarır. |
| [getFileEntries()](#getFileEntries--) | xz arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) tipindeki girdileri alır. |
| [getFormat()](#getFormat--) | Arşiv biçimini alır. |
| [getLength()](#getLength--) | Girdinin uzunluğunu bayt cinsinden alır. |
| [getName()](#getName--) | Arşiv içindeki girişin adını alır. |
| [getUncompressedSize()](#getUncompressedSize--) | Dosya verisinin sıkıştırılmamış boyutunu bayt cinsinden alır. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | xz arşivini verilen akışa kaydeder. |
| [save(String destinationFileName)](#save-java.lang.String-) | xz arşivini verilen hedef dosyaya kaydeder. |
| [setSource(File file)](#setSource-java.io.File-) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
### XzArchive() {#XzArchive--}
```
public XzArchive()
```


Yeni bir [XzArchive](../../com.aspose.zip/xzarchive) sınıfı örneği başlatır ve arşivi xz formatında oluşturur.

### XzArchive(XzArchiveSettings settings) {#XzArchive-com.aspose.zip.XzArchiveSettings-}
```
public XzArchive(XzArchiveSettings settings)
```


Yeni bir [XzArchive](../../com.aspose.zip/xzarchive) sınıfı örneği başlatır ve arşivi xz formatında oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | belirli xz arşivi ayarları kümesi: sözlük boyutu, blok boyutu, kontrol türü |

### XzArchive(InputStream source) {#XzArchive-java.io.InputStream-}
```
public XzArchive(InputStream source)
```


Yeni bir [XzArchive](../../com.aspose.zip/xzarchive) sınıfı örneği başlatır ve açma işlemi için hazırlar.

Bu yapıcı sıkıştırmayı açmaz. Sıkıştırmayı açmak için [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | java.io.InputStream | arşivin kaynağı |

### XzArchive(InputStream source, XzLoadOptions options) {#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(InputStream source, XzLoadOptions options)
```


Yeni bir [XzArchive](../../com.aspose.zip/xzarchive) sınıfı örneği başlatır ve açma işlemi için hazırlar.

Bu yapıcı sıkıştırmayı açmaz. Sıkıştırmayı açmak için [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | java.io.InputStream | arşivin kaynağı |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) | Arşivi yüklemek için seçenekler. |

### XzArchive(String path) {#XzArchive-java.lang.String-}
```
public XzArchive(String path)
```


Yeni bir [XzArchive](../../com.aspose.zip/xzarchive) sınıfı örneği başlatır ve açma işlemi için hazırlar.

Bu yapıcı sıkıştırmayı açmaz. Sıkıştırmayı açmak için [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | arşivin kaynağına yol |

### XzArchive(String path, XzLoadOptions options) {#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(String path, XzLoadOptions options)
```


Yeni bir [XzArchive](../../com.aspose.zip/xzarchive) sınıfı örneği başlatır ve açma işlemi için hazırlar.

Bu yapıcı sıkıştırmayı açmaz. Sıkıştırmayı açmak için [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | arşivin kaynağına yol |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) |  |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


xz arşivini bir dosyaya çıkarır.

```

``````

try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
try (XzArchive archive = new XzArchive(xzFile)) {
archive.extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts xz archive to a stream.

```

``````

     try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (XzArchive archive = new XzArchive(xzFile)) {
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


xz arşivini yol belirterek bir dosyaya çıkarır.

```

``````

try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
try (XzArchive archive = new XzArchive(xzFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | path to file which will store decompressed data |

**Returns:**
java.io.File - java.io.File instance containing extracted data
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive
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


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within archive.

**Returns:**
java.lang.String - the name of the entry within archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the file data in bytes.

**Returns:**
long - the uncompressed size of the file data in bytes
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves xz archive to the stream provided.

```

``````

     try (FileOutputStream xzFile = new FileOutputStream("archive.xz")) {
         try (XzArchive archive = new XzArchive()) {
             archive.setSource("data.bin");
             archive.save(xzFile);
         }
     } catch (IOException ex) {
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


xz arşivini verilen hedef dosyaya kaydeder.

```

``````

try (XzArchive archive = new XzArchive()) {
archive.setSource(new File("data.bin"));
archive.save("result.xz");
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

     try (XzArchive archive = new XzArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosya | java.io.File | giriş akışı olarak açılacak dosya |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Arşiv içinde sıkıştırılacak içeriği ayarlar.

```

``````

try (XzArchive archive = new XzArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.xz");
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

     try (XzArchive archive = new XzArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourcePath | java.lang.String | giriş akışı olarak açılacak dosyanın yolu |

