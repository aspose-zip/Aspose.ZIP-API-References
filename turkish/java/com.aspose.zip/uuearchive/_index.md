---
title: "UueArchive"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bu sınıf uuencoded dosyasını temsil eder."
type: docs
weight: 128
url: /tr/java/com.aspose.zip/uuearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class UueArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Bu sınıf uuencoded dosyasını temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [UueArchive()](#UueArchive--) | Kodlama için hazırlanmış [UueArchive](../../com.aspose.zip/uuearchive) sınıfının yeni bir örneğini başlatır. |
| [UueArchive(InputStream sourceStream)](#UueArchive-java.io.InputStream-) | Kod çözme için hazırlanmış [UueArchive](../../com.aspose.zip/uuearchive) sınıfının yeni bir örneğini başlatır. |
| [UueArchive(String path)](#UueArchive-java.lang.String-) | [UueArchive](../../com.aspose.zip/uuearchive) sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Arşivi sağlanan akıma çıkarır. |
| [extract(String path)](#extract-java.lang.String-) | Arşivi belirtilen yola dosya olarak çıkarır. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Arşivin içeriğini sağlanan dizine çıkarır. |
| [getFileEntries()](#getFileEntries--) | uue arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) tipindeki girdileri alır. |
| [getFormat()](#getFormat--) | Arşiv biçimini alır. |
| [getLength()](#getLength--) | Uzunluğu alır. |
| [getName()](#getName--) | Orijinal dosyanın adı. |
| [open()](#open--) | Arşivi kod çözme için açar ve arşiv içeriğiyle bir akış sağlar. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Sağlanan akışa arşivi kaydeder. |
| [save(OutputStream outputStream, UueSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.UueSaveOptions-) | Sağlanan akışa arşivi kaydeder. |
| [save(String destinationFileName)](#save-java.lang.String-) | Arşivi sağlanan hedef dosyaya kaydeder. |
| [save(String destinationFileName, UueSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.UueSaveOptions-) | Arşivi sağlanan hedef dosyaya kaydeder. |
| [setSource(File file)](#setSource-java.io.File-) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Arşiv içinde kodlanacak içeriği ayarlar. |
| [setSource(String path)](#setSource-java.lang.String-) | Arşiv içinde kodlanacak içeriği ayarlar. |
### UueArchive() {#UueArchive--}
```
public UueArchive()
```


Kodlama için hazırlanmış [UueArchive](../../com.aspose.zip/uuearchive) sınıfının yeni bir örneğini başlatır.

Aşağıdaki örnek, bir dosyanın uuencode nasıl yapılacağını gösterir.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(\"data.bin\");
archive.save(\"archive.uue\");
}
 
```



### UueArchive(InputStream sourceStream) {#UueArchive-java.io.InputStream-}
```
public UueArchive(InputStream sourceStream)
```


Initializes a new instance of the [UueArchive](../../com.aspose.zip/uuearchive) class prepared for decoding.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (UueArchive archive = new UueArchive(new FileInputStream("archive.001"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

Bu yapıcı kod çözmez. Açmak için [open()](../../com.aspose.zip/uuearchive\#open--) yöntemine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceStream | java.io.InputStream | arşivin kaynağı |

### UueArchive(String path) {#UueArchive-java.lang.String-}
```
public UueArchive(String path)
```


[UueArchive](../../com.aspose.zip/uuearchive) sınıfının yeni bir örneğini başlatır.

Yolu belirterek bir arşivi dosyadan açın ve bir `MemoryStream`'e kod çözün.

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (UueArchive archive = new UueArchive(new FileInputStream(\"archive.uue\"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decode. See [open()](../../com.aspose.zip/uuearchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

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

     try (UueArchive archive = new UueArchive("archive.uue")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hedef | java.io.OutputStream | hedef akışı |

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
java.io.File - çıkarılan dosyanın bilgisi
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


uue arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) tipindeki girdileri alır.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - uue arşivini oluşturan [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) tipindeki girdiler
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
### open() {#open--}
```
public final InputStream open()
```


Arşivi kod çözme için açar ve arşiv içeriğiyle bir akış sağlar.

Kullanım:

```

``````

try (InputStream decompressed = archive.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the archive
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Write compressed data to http response stream.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(outputStream);
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| outputStream | java.io.OutputStream | hedef akışı |

### save(OutputStream outputStream, UueSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.UueSaveOptions-}
```
public final void save(OutputStream outputStream, UueSaveOptions saveOptions)
```


Sağlanan akışa arşivi kaydeder.

Sıkıştırılmış veriyi http yanıt akışına yazın.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new File("data.bin"));
archive.save(outputStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream |
| saveOptions | [UueSaveOptions](../../com.aspose.zip/uuesaveoptions) | options for the archive saving |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves the archive to the destination file provided.

Write encoded data to file.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.uue");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destinationFileName | java.lang.String | oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |

### save(String destinationFileName, UueSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.UueSaveOptions-}
```
public final void save(String destinationFileName, UueSaveOptions saveOptions)
```


Arşivi sağlanan hedef dosyaya kaydeder.

Kodlanmış veriyi dosyaya yazın.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new File("data.bin"));
archive.save(\"data.uue\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| saveOptions | [UueSaveOptions](../../com.aspose.zip/uuesaveoptions) | options for the archive saving |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.uue");
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


Arşiv içinde kodlanacak içeriği ayarlar.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save(\"archive.uue\");
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


Sets the content to be encoded within the archive.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.uue");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | kodlanacak dosyanın yolu |

