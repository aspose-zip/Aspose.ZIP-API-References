---
title: "SevenZipArchiveEntry"
second_title: "Aspose.ZIP for Java API Referansı"
description: "7z arşivi içinde tek bir dosyayı temsil eder."
type: docs
weight: 105
url: /tr/java/com.aspose.zip/sevenziparchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class SevenZipArchiveEntry implements IArchiveFileEntry
```

7z arşivi içinde tek bir dosyayı temsil eder.

Bir [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) örneğini [SevenZipArchiveEntryEncrypted](../../com.aspose.zip/sevenziparchiveentryencrypted) tipine dönüştürerek girişin şifreli olup olmadığını belirleyin.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Girdiyi sağlanan akıma çıkarır. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Girdiyi sağlanan akıma çıkarır. |
| [extract(String path)](#extract-java.lang.String-) | Girdiyi sağlanan yola göre dosya sistemine çıkarır. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Girdiyi sağlanan yola göre dosya sistemine çıkarır. |
| [getCompressedSize()](#getCompressedSize--) | Sıkıştırılmış dosyanın boyutunu alır. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Ham akışın bir bölümü sıkıştırıldığında tetiklenen bir olayı alır. |
| [getCompressionSettings()](#getCompressionSettings--) | Sıkıştırma veya açma ayarlarını alır. |
| [getLength()](#getLength--) | Uzunluğu alır. |
| [getModificationTime()](#getModificationTime--) | Son değiştirilme tarih ve saatini alır. |
| [getName()](#getName--) | Arşiv içindeki girdinin adını alır. |
| [getUncompressedSize()](#getUncompressedSize--) | Orijinal dosyanın boyutunu alır. |
| [isDirectory()](#isDirectory--) | Girdinin bir dizin olup olmadığını gösteren değeri alır. |
| [open()](#open--) | Girdiyi çıkarmak için açar ve giriş içeriğiyle bir akış sağlar. |
| [open(String password)](#open-java.lang.String-) | Girdiyi çıkarmak için açar ve giriş içeriğiyle bir akış sağlar. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Ham akışın bir bölümü sıkıştırıldığında tetiklenen bir olayı ayarlar. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Girdiyi sağlanan akıma çıkarır.

Şifre ile zip arşivindeki bir girdiyi çıkar.

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.

Extract an entry of zip archive with password.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.getEntries().get(0).extract(httpResponseStream);
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hedef | java.io.OutputStream | hedef akış. Yazılabilir olmalıdır |
| password | java.lang.String | Şifre çözme için isteğe bağlı parola |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Girdiyi sağlanan yola göre dosya sistemine çıkarır.

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.getEntries().get(0).extract("data.bin");
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

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | hedef dosyanın yolu. Dosya zaten mevcutsa, üzerine yazılacaktır. |
| password | java.lang.String | Şifre çözme için isteğe bağlı parola |

**Returns:**
java.io.File - çıkarılan dosyanın dosya bilgisi
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

Event sender is an [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) instance.

Does not invoke in solid mode and in multithreaded mode for LZMA2 entries.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression
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


Gets the name of the entry within the archive.

**Returns:**
java.lang.String - the name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the size of the original file.

**Returns:**
long - the size of the original file
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with entry content.

Usage:

```

``````

     SevenZipArchive archive = new SevenZipArchive("archive.7z");
     SevenZipArchiveEntry entry = archive.getEntries().get(0);
     try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
         try (InputStream decompressed = entry.open()) {
             byte[] buffer = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
                 fileStream.write(buffer, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

Akıştan okuyarak dosyanın orijinal içeriğini alın. Örnekler bölümüne bakın.

**Returns:**
java.io.InputStream - girişin içeriğini temsil eden akış
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Girdiyi çıkarmak için açar ve giriş içeriğiyle bir akış sağlar.

Kullanım:

```

``````

SevenZipArchive archive = new SevenZipArchive("archive.7z");
SevenZipArchiveEntry entry = archive.getEntries().get(0);
try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
try (InputStream decompressed = entry.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | optional password for decryption |

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
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

Olay göndericisi bir [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) örneğidir.

LZMA2 girişleri için katı modda ve çok iş parçacıklı modda çağrılmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | ham akışın bir bölümü sıkıştırıldığında tetiklenen bir olay |

