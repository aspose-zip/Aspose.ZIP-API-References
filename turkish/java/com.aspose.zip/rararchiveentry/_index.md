---
title: "RarArchiveEntry"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Arşiv içinde tek bir dosyayı temsil eder."
type: docs
weight: 98
url: /tr/java/com.aspose.zip/rararchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class RarArchiveEntry implements IArchiveFileEntry
```

Arşiv içinde tek bir dosyayı temsil eder.

Bir [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) örneğini [RarArchiveEntryEncrypted](../../com.aspose.zip/rararchiveentryencrypted) tipine dönüştürerek girdinin şifrelenip şifrelenmediğini belirleyin.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Girdiyi sağlanan akıma çıkarır. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Girdiyi sağlanan akıma çıkarır. |
| [extract(String path)](#extract-java.lang.String-) | Girdiyi sağlanan yola göre dosya sistemine çıkarır. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Girdiyi sağlanan yola göre dosya sistemine çıkarır. |
| [getCompressedSize()](#getCompressedSize--) | Sıkıştırılmış dosyanın boyutunu alır. |
| [getCreationTime()](#getCreationTime--) | Oluşturulma tarih ve saatini alır. |
| [getExtractionProgressed()](#getExtractionProgressed--) | Ham akışın bir kısmı çıkarıldığında tetiklenen bir olayı alır. |
| [getLastAccessTime()](#getLastAccessTime--) | Son erişim tarih ve saatini alır. |
| [getLength()](#getLength--) | Uzunluğu alır. |
| [getModificationTime()](#getModificationTime--) | Son değiştirilme tarih ve saatini alır. |
| [getName()](#getName--) | Arşiv içindeki girdinin adını alır. |
| [getUncompressedSize()](#getUncompressedSize--) | Orijinal dosyanın boyutunu alır. |
| [isDirectory()](#isDirectory--) | Girdinin bir dizin olup olmadığını gösteren değeri alır. |
| [open()](#open--) | Girdiyi çıkarmak için açar ve sıkıştırması çözülmüş içerikle bir akış sağlar. |
| [open(String password)](#open-java.lang.String-) | Girdiyi çıkarmak için açar ve sıkıştırması çözülmüş içerikle bir akış sağlar. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Ham akışın bir kısmı çıkarıldığında tetiklenen bir olayı ayarlar. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Girdiyi sağlanan akıma çıkarır.


Şifreyle bir rar arşivi girdisini çıkar.

```

``````

try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
try (RarArchive archive = new RarArchive(rarFile)) {
archive.getEntries().get(0).extract(outputStream, "p@s$");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.


Extract an entry of rar archive with password.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
            archive.getEntries().get(0).extract(outputStream, "p@s$");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hedef | java.io.OutputStream | Hedef akış. Yazılabilir olmalıdır. |
| password | java.lang.String | Şifre çözme için isteğe bağlı şifre. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Girdiyi sağlanan yola göre dosya sistemine çıkarır.


Rar arşivinden iki girdi çıkar.

```

``````

try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
try (RarArchive archive = new RarArchive(rarFile)) {
archive.getEntries().get(0).extract("first.bin", "pass");
archive.getEntries().get(1).extract("second.bin", "pass");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.


Extract two entries of rar archive.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
            archive.getEntries().get(0).extract("first.bin", "pass");
            archive.getEntries().get(1).extract("second.bin", "pass");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | Hedef dosyanın yolu. Dosya zaten mevcutsa, üzerine yazılacaktır. |
| password | java.lang.String | Şifre çözme için isteğe bağlı şifre. |

**Returns:**
java.io.File - çıkarılan dosyanın dosya bilgisi
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Sıkıştırılmış dosyanın boyutunu alır.

**Returns:**
long - sıkıştırılmış dosyanın boyutu
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Oluşturulma tarih ve saatini alır.

**Returns:**
java.util.Date - oluşturulma tarih ve saati.
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressEventArgs> getExtractionProgressed()
```


Ham akışın bir kısmı çıkarıldığında tetiklenen bir olayı alır.

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
}
});
 
```

Event sender is an [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Gets last access date and time.

**Returns:**
java.util.Date - last access date and time.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length.
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within the archive.

**Returns:**
java.lang.String - the name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the size of the original file.

**Returns:**
long - the size of the original file.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory.
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with decompressed entry content.


Usage:

```

``````

    InputStream decompressed = entry.open();
    byte[] buffer = new byte[8192];
    int bytesRead;
    while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
        fileStream.write(buffer, 0, bytesRead);
 
```

Akıştan okuyarak dosyanın orijinal içeriğini alın. Örnekler bölümüne bakın.

**Returns:**
java.io.InputStream - Girdinin içeriğini temsil eden akış.
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Girdiyi çıkarmak için açar ve sıkıştırması çözülmüş içerikle bir akış sağlar.


Kullanım:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
fileStream.write(buffer, 0, bytesRead);
 
```

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Optional password for decryption. It can also be set within [RarArchiveLoadOptions.setDecryptionPassword(String)](../../com.aspose.zip/rararchiveloadoptions\#setDecryptionPassword-String-). |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream extracted.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

Olay göndericisi bir [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) örneğidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | ham akışın bir bölümü çıkarıldığında tetiklenen bir olay. |

