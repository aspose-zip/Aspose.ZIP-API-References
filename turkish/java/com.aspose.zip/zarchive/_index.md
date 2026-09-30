---
title: "ZArchive"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bu sınıf bir Z sıkıştırma arşiv dosyasını temsil eder."
type: docs
weight: 153
url: /tr/java/com.aspose.zip/zarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ZArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

Bu sınıf bir Z (compress) arşiv dosyasını temsil eder. Z arşivlerini oluşturmak veya çıkarmak için kullanın.

Bakınız [Z Compressed File Format ][Z Compressed File Format]


[Z Compressed File Format]: https://docs.fileformat.com/compression/z/
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ZArchive()](#ZArchive--) | Sıkıştırma için hazırlanmış [ZArchive](../../com.aspose.zip/zarchive) sınıfının yeni bir örneğini başlatır. |
| [ZArchive(InputStream source)](#ZArchive-java.io.InputStream-) | Açma için hazırlanmış [ZArchive](../../com.aspose.zip/zarchive) sınıfının yeni bir örneğini başlatır. |
| [ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)](#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-) | Açma için hazırlanmış [ZArchive](../../com.aspose.zip/zarchive) sınıfının yeni bir örneğini başlatır. |
| [ZArchive(String path)](#ZArchive-java.lang.String-) | Açma için hazırlanmış [ZArchive](../../com.aspose.zip/zarchive) sınıfının yeni bir örneğini başlatır. |
| [ZArchive(String path, ZArchiveLoadOptions loadOptions)](#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-) | Açma için hazırlanmış [ZArchive](../../com.aspose.zip/zarchive) sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Z arşivini bir dosyaya çıkarır. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Z arşivini bir akışa çıkarır. |
| [extract(String path)](#extract-java.lang.String-) | Z arşivini yol belirterek bir dosyaya çıkarır. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Arşivin içeriğini sağlanan dizine çıkarır. |
| [getFileEntries()](#getFileEntries--) | Z arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) tipindeki girişleri alır. |
| [getFormat()](#getFormat--) | Arşiv biçimini alır. |
| [getLength()](#getLength--) | Girdinin uzunluğunu bayt cinsinden alır. |
| [getName()](#getName--) | Arşiv içindeki girişin adını alır. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Z arşivini sağlanan akışa kaydeder. |
| [save(OutputStream output, ZArchiveSaveOptions settings)](#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-) | Z arşivini sağlanan akışa kaydeder. |
| [save(String destinationFileName)](#save-java.lang.String-) | Z arşivini sağlanan hedef dosyaya kaydeder. |
| [save(String destinationFileName, ZArchiveSaveOptions settings)](#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-) | Z arşivini sağlanan hedef dosyaya kaydeder. |
| [setSource(File file)](#setSource-java.io.File-) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
### ZArchive() {#ZArchive--}
```
public ZArchive()
```


Sıkıştırma için hazırlanmış [ZArchive](../../com.aspose.zip/zarchive) sınıfının yeni bir örneğini başlatır.

### ZArchive(InputStream source) {#ZArchive-java.io.InputStream-}
```
public ZArchive(InputStream source)
```


Açma için hazırlanmış [ZArchive](../../com.aspose.zip/zarchive) sınıfının yeni bir örneğini başlatır.

Bu yapıcı açma işlemi yapmaz. Açma için [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | java.io.InputStream | arşivin kaynağı |

### ZArchive(InputStream source, ZArchiveLoadOptions loadOptions) {#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)
```


Açma için hazırlanmış [ZArchive](../../com.aspose.zip/zarchive) sınıfının yeni bir örneğini başlatır.

Bu yapıcı açma işlemi yapmaz. Açma için [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | java.io.InputStream | arşivin kaynağı |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | arşivi yüklemek için seçenekler |

### ZArchive(String path) {#ZArchive-java.lang.String-}
```
public ZArchive(String path)
```


Açma için hazırlanmış [ZArchive](../../com.aspose.zip/zarchive) sınıfının yeni bir örneğini başlatır.

Bu yapıcı açma işlemi yapmaz. Açma için [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | arşivin kaynağına giden yol |

### ZArchive(String path, ZArchiveLoadOptions loadOptions) {#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(String path, ZArchiveLoadOptions loadOptions)
```


Açma için hazırlanmış [ZArchive](../../com.aspose.zip/zarchive) sınıfının yeni bir örneğini başlatır.

Bu yapıcı açma işlemi yapmaz. Açma için [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | arşivin kaynağına giden yol |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | arşivi yüklemek için seçenekler |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Z arşivini bir dosyaya çıkarır.

```

``````

try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
try (ZArchive archive = new ZArchive(zFile)) {
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


Extracts Z archive to a stream.

```

``````

     try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (ZArchive archive = new ZArchive(zFile)) {
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


Z arşivini yol belirterek bir dosyaya çıkarır.

```

``````

try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
try (ZArchive archive = new ZArchive(zFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to file which will store decompressed data |

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
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive
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
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves Z archive to the stream provided.

```

``````

     try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
         try (ZArchive archive = new ZArchive()) {
             archive.setSource("data.bin");
             archive.save(zFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| output | java.io.OutputStream | hedef akış |

### save(OutputStream output, ZArchiveSaveOptions settings) {#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(OutputStream output, ZArchiveSaveOptions settings)
```


Z arşivini sağlanan akışa kaydeder.

```

``````

try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
try (ZArchive archive = new ZArchive()) {
archive.setSource(\"data.bin\");
archive.save(zFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves Z archive to the destination file provided.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationFileName | java.lang.String | oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |

### save(String destinationFileName, ZArchiveSaveOptions settings) {#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(String destinationFileName, ZArchiveSaveOptions settings)
```


Z arşivini sağlanan hedef dosyaya kaydeder.

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new File("data.bin"));
archive.save("data.bin.Z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosya | java.io.File | giriş akışı olarak açılacak dosya bilgisi |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Arşiv içinde sıkıştırılacak içeriği ayarlar.

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save("archive.Z");
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

     try (ZArchive archive = new ZArchive()) {
         archive.setSource("data.bin");
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourcePath | java.lang.String | giriş akışı olarak açılacak dosyanın yolu |

