---
title: "ArchiveEntry"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Arşiv içinde tek bir dosyayı temsil eder."
type: docs
weight: 27
url: /tr/java/com.aspose.zip/archiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class ArchiveEntry implements IArchiveFileEntry
```

Arşiv içinde tek bir dosyayı temsil eder.

Bir [ArchiveEntry](../../com.aspose.zip/archiveentry) örneğini [ArchiveEntryEncrypted](../../com.aspose.zip/archiveentryencrypted) tipine dönüştürerek girdinin şifreli olup olmadığını belirleyin.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Girdiyi sağlanan akıma çıkarır. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Girdiyi sağlanan akıma çıkarır. |
| [extract(String path)](#extract-java.lang.String-) | Girdiyi sağlanan yola göre dosya sistemine çıkarır. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Girdiyi sağlanan yola göre dosya sistemine çıkarır. |
| [getComment()](#getComment--) | Arşiv içindeki girdinin yorumunu alır. |
| [getCompressedSize()](#getCompressedSize--) | Sıkıştırılmış dosyanın boyutunu alır. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Ham akışın bir bölümü sıkıştırıldığında tetiklenen bir olayı alır. |
| [getCompressionSettings()](#getCompressionSettings--) | Sıkıştırma veya açma ayarlarını alır. |
| [getDataSource()](#getDataSource--) | Girdi arşive eklendiyse, çıkarılmadan kaynak. |
| [getExtractionProgressed()](#getExtractionProgressed--) | Ham akışın bir kısmı çıkarıldığında tetiklenen bir olayı alır. |
| [getLength()](#getLength--) | Uzunluğu alır. |
| [getModificationTime()](#getModificationTime--) | Son değiştirilme tarih ve saatini alır. |
| [getName()](#getName--) | Arşiv içindeki girdinin adını alır. |
| [getUncompressedSize()](#getUncompressedSize--) | Orijinal dosyanın boyutunu alır. |
| [isDirectory()](#isDirectory--) | Girdinin bir dizin olup olmadığını gösteren değeri alır. |
| [open()](#open--) | Girdiyi çıkarmak için açar ve sıkıştırması çözülmüş içerikle bir akış sağlar. |
| [open(String password)](#open-java.lang.String-) | Girdiyi çıkarmak için açar ve sıkıştırması çözülmüş içerikle bir akış sağlar. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Ham akışın bir bölümü sıkıştırıldığında tetiklenen bir olayı ayarlar. |
| [setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | Ham akışın bir kısmı çıkarıldığında tetiklenen bir olayı ayarlar. |
| [setModificationTime(Date value)](#setModificationTime-java.util.Date-) | Son değiştirilme tarih ve saatini ayarlar. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Girdiyi sağlanan akıma çıkarır.

Şifre ile zip arşivindeki bir girdiyi çıkar.

```

``````

try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
try (Archive archive = new Archive(zipFile)) {
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

Extract an entry of zip archive with password.

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
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

Her biri kendi şifresiyle ZIP arşivinden iki girdi çıkar.

```

``````

try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
try (Archive archive = new Archive(zipFile)) {
archive.getEntries().get(0).extract("first.bin", "first_pass");
archive.getEntries().get(1).extract("second.bin", "second_pass");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to destination file. If the file already exists, it will be overwritten. |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of ZIP archive, each with own password

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
            archive.getEntries().get(0).extract("first.bin", "first_pass");
            archive.getEntries().get(1).extract("second.bin", "second_pass");
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
### getComment() {#getComment--}
```
public final String getComment()
```


Arşiv içindeki girdinin yorumunu alır.

**Returns:**
java.lang.String - arşiv içindeki girdinin yorumu
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Sıkıştırılmış dosyanın boyutunu alır.

**Returns:**
long - sıkıştırılmış dosyanın boyutu
### getCompressionProgressed() {#getCompressionProgressed--}
```
public final Event<ProgressEventArgs> getCompressionProgressed()
```


Ham akışın bir bölümü sıkıştırıldığında tetiklenen bir olayı alır.

```

``````

archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression.
### getDataSource() {#getDataSource--}
```
public final InputStream getDataSource()
```


Source for the entry if the entry was added to the archive, not extracted.

Before assigned, the source is null. This source may be assigned within `Archive.save` method in some cases.

**Returns:**
java.io.InputStream - the source for the entry
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressCancelEventArgs> getExtractionProgressed()
```


Gets an event that is raised when a portion of raw stream extracted.

In this sample event handler is used for calculation the share of proceeded size in percents.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

Bu örnekte, girdinin ilk yüz MB'ı çıkarıldıktan sonra iptal için olay işleyicisi kullanılır.

```

``````

a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance. It is possible to cancel extraction.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time
### getName() {#getName--}
```
public final String getName()
```


Gets name of the entry within the archive.

**Returns:**
java.lang.String - name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file
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

Dosyanın orijinal içeriğini elde etmek için akıştan okuyun.

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
| password | java.lang.String | Optional password for decryption. |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

``````

    archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```

Olay göndericisi bir [ArchiveEntry](../../com.aspose.zip/archiveentry) örneğidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | ham akışın bir bölümü sıkıştırıldığında tetiklenen bir olay |

### setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


Ham akışın bir kısmı çıkarıldığında tetiklenen bir olayı ayarlar.

Bu örnekte olay işleyicisi, işlenen boyutun yüzde olarak payını hesaplamak için kullanılır.

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
 
```

In this sample event handler is used for cancellation after the first hundred of Mb of entry was extracted.

```

``````

 a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

Event göndericisi bir [ArchiveEntry](../../com.aspose.zip/archiveentry) örneğidir. Çıkarma işlemini iptal etmek mümkündür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | ham akışın bir bölümü çıkarıldığında tetiklenen bir olay. |

### setModificationTime(Date value) {#setModificationTime-java.util.Date-}
```
public final void setModificationTime(Date value)
```


Son değiştirilme tarih ve saatini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | son değiştirilme tarihi ve saati |

