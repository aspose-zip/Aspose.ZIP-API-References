---
title: "RarArchiveEntry"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Mewakili file tunggal dalam arsip."
type: docs
weight: 98
url: /id/java/com.aspose.zip/rararchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class RarArchiveEntry implements IArchiveFileEntry
```

Mewakili file tunggal dalam arsip.

Cast sebuah instance [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) ke [RarArchiveEntryEncrypted](../../com.aspose.zip/rararchiveentryencrypted) untuk menentukan apakah entri terenkripsi atau tidak.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Mengekstrak entri ke aliran yang disediakan. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Mengekstrak entri ke aliran yang disediakan. |
| [extract(String path)](#extract-java.lang.String-) | Mengekstrak entri ke sistem file menggunakan jalur yang disediakan. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Mengekstrak entri ke sistem file menggunakan jalur yang disediakan. |
| [getCompressedSize()](#getCompressedSize--) | Mendapatkan ukuran file terkompresi. |
| [getCreationTime()](#getCreationTime--) | Mendapatkan tanggal dan waktu pembuatan. |
| [getExtractionProgressed()](#getExtractionProgressed--) | Mendapatkan sebuah peristiwa yang dipicu ketika sebagian aliran mentah diekstrak. |
| [getLastAccessTime()](#getLastAccessTime--) | Mendapatkan tanggal dan waktu akses terakhir. |
| [getLength()](#getLength--) | Mendapatkan panjang. |
| [getModificationTime()](#getModificationTime--) | Mendapatkan tanggal dan waktu terakhir dimodifikasi. |
| [getName()](#getName--) | Mendapatkan nama entri di dalam arsip. |
| [getUncompressedSize()](#getUncompressedSize--) | Mendapatkan ukuran file asli. |
| [isDirectory()](#isDirectory--) | Mendapatkan nilai yang menunjukkan apakah entri mewakili sebuah direktori. |
| [open()](#open--) | Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri yang didekompresi. |
| [open(String password)](#open-java.lang.String-) | Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri yang didekompresi. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Menetapkan sebuah peristiwa yang dipicu ketika sebagian aliran mentah diekstrak. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Mengekstrak entri ke aliran yang disediakan.


Ekstrak sebuah entri arsip rar dengan kata sandi.

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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tujuan | java.io.OutputStream | Aliran tujuan. Harus dapat ditulis. |
| password | java.lang.String | Kata sandi opsional untuk dekripsi. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Mengekstrak entri ke sistem file menggunakan jalur yang disediakan.


Ekstrak dua entri arsip rar.

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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | Jalur ke file tujuan. Jika file sudah ada, akan ditimpa. |
| password | java.lang.String | Kata sandi opsional untuk dekripsi. |

**Returns:**
java.io.File - informasi file dari file yang diekstrak
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Mendapatkan ukuran file terkompresi.

**Returns:**
long - ukuran file terkompresi
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Mendapatkan tanggal dan waktu pembuatan.

**Returns:**
java.util.Date - tanggal dan waktu pembuatan.
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressEventArgs> getExtractionProgressed()
```


Mendapatkan sebuah peristiwa yang dipicu ketika sebagian aliran mentah diekstrak.

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

Baca dari aliran untuk mendapatkan konten asli file. Lihat bagian contoh.

**Returns:**
java.io.InputStream - Aliran yang mewakili isi entri.
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri yang didekompresi.


Penggunaan:

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

Pengirim Event adalah sebuah instance [RarArchiveEntry](../../com.aspose.zip/rararchiveentry).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | sebuah event yang dipicu ketika sebagian aliran mentah diekstrak. |

