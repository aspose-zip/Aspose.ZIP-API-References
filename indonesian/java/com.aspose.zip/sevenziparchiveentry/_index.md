---
title: "SevenZipArchiveEntry"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Mewakili satu file dalam arsip 7z."
type: docs
weight: 105
url: /id/java/com.aspose.zip/sevenziparchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class SevenZipArchiveEntry implements IArchiveFileEntry
```

Mewakili satu file dalam arsip 7z.

Cast sebuah instance [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) ke [SevenZipArchiveEntryEncrypted](../../com.aspose.zip/sevenziparchiveentryencrypted) untuk menentukan apakah entri terenkripsi atau tidak.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Mengekstrak entri ke aliran yang disediakan. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Mengekstrak entri ke aliran yang disediakan. |
| [extract(String path)](#extract-java.lang.String-) | Mengekstrak entri ke sistem file menggunakan jalur yang disediakan. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Mengekstrak entri ke sistem file menggunakan jalur yang disediakan. |
| [getCompressedSize()](#getCompressedSize--) | Mendapatkan ukuran file terkompresi. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Mendapatkan peristiwa yang dipicu ketika sebagian aliran mentah dikompresi. |
| [getCompressionSettings()](#getCompressionSettings--) | Mendapatkan pengaturan untuk kompresi atau dekompresi. |
| [getLength()](#getLength--) | Mendapatkan panjang. |
| [getModificationTime()](#getModificationTime--) | Mendapatkan tanggal dan waktu terakhir dimodifikasi. |
| [getName()](#getName--) | Mendapatkan nama entri di dalam arsip. |
| [getUncompressedSize()](#getUncompressedSize--) | Mendapatkan ukuran file asli. |
| [isDirectory()](#isDirectory--) | Mendapatkan nilai yang menunjukkan apakah entri mewakili sebuah direktori. |
| [open()](#open--) | Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri. |
| [open(String password)](#open-java.lang.String-) | Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Mengatur peristiwa yang dipicu ketika sebagian aliran mentah dikompresi. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Mengekstrak entri ke aliran yang disediakan.

Ekstrak sebuah entri arsip zip dengan kata sandi.

```

``````

coba (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tujuan | java.io.OutputStream | stream tujuan. Harus dapat ditulis |
| password | java.lang.String | kata sandi opsional untuk dekripsi |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Mengekstrak entri ke sistem file menggunakan jalur yang disediakan.

```

``````

coba (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur ke file tujuan. Jika file sudah ada, akan ditimpa. |
| password | java.lang.String | kata sandi opsional untuk dekripsi |

**Returns:**
java.io.File - informasi file dari file yang diekstrak
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Mendapatkan ukuran file terkompresi.

**Returns:**
long - ukuran file terkompresi
### getCompressionProgressed() {#getCompressionProgressed--}
```
public final Event<ProgressEventArgs> getCompressionProgressed()
```


Mendapatkan peristiwa yang dipicu ketika sebagian aliran mentah dikompresi.

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

Baca dari aliran untuk mendapatkan konten asli file. Lihat bagian contoh.

**Returns:**
java.io.InputStream - aliran yang mewakili isi entri
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri.

Penggunaan:

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

Pengirim peristiwa adalah sebuah instance [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry).

Tidak dipanggil dalam mode solid dan dalam mode multithreaded untuk entri LZMA2.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | sebuah event yang dipicu ketika sebagian aliran mentah dikompresi |

