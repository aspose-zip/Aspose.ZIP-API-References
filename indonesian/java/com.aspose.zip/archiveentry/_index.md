---
title: "ArchiveEntry"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Mewakili file tunggal dalam arsip."
type: docs
weight: 27
url: /id/java/com.aspose.zip/archiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class ArchiveEntry implements IArchiveFileEntry
```

Mewakili file tunggal dalam arsip.

Cast sebuah instance [ArchiveEntry](../../com.aspose.zip/archiveentry) ke [ArchiveEntryEncrypted](../../com.aspose.zip/archiveentryencrypted) untuk menentukan apakah entri terenkripsi atau tidak.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Mengekstrak entri ke aliran yang disediakan. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Mengekstrak entri ke aliran yang disediakan. |
| [extract(String path)](#extract-java.lang.String-) | Mengekstrak entri ke sistem file menggunakan jalur yang disediakan. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Mengekstrak entri ke sistem file menggunakan jalur yang disediakan. |
| [getComment()](#getComment--) | Mendapatkan komentar dari entri dalam arsip. |
| [getCompressedSize()](#getCompressedSize--) | Mendapatkan ukuran file terkompresi. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Mendapatkan peristiwa yang dipicu ketika sebagian aliran mentah dikompresi. |
| [getCompressionSettings()](#getCompressionSettings--) | Mendapatkan pengaturan untuk kompresi atau dekompresi. |
| [getDataSource()](#getDataSource--) | Sumber untuk entri jika entri ditambahkan ke arsip, bukan diekstrak. |
| [getExtractionProgressed()](#getExtractionProgressed--) | Mendapatkan sebuah peristiwa yang dipicu ketika sebagian aliran mentah diekstrak. |
| [getLength()](#getLength--) | Mendapatkan panjang. |
| [getModificationTime()](#getModificationTime--) | Mendapatkan tanggal dan waktu terakhir dimodifikasi. |
| [getName()](#getName--) | Mendapatkan nama entri dalam arsip. |
| [getUncompressedSize()](#getUncompressedSize--) | Mendapatkan ukuran file asli. |
| [isDirectory()](#isDirectory--) | Mendapatkan nilai yang menunjukkan apakah entri mewakili sebuah direktori. |
| [open()](#open--) | Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri yang didekompresi. |
| [open(String password)](#open-java.lang.String-) | Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri yang didekompresi. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Mengatur peristiwa yang dipicu ketika sebagian aliran mentah dikompresi. |
| [setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | Menetapkan sebuah peristiwa yang dipicu ketika sebagian aliran mentah diekstrak. |
| [setModificationTime(Date value)](#setModificationTime-java.util.Date-) | Menetapkan tanggal dan waktu terakhir dimodifikasi. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Mengekstrak entri ke aliran yang disediakan.

Ekstrak sebuah entri arsip zip dengan kata sandi.

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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tujuan | java.io.OutputStream | Aliran tujuan. Harus dapat ditulis. |
| password | java.lang.String | Kata sandi opsional untuk dekripsi. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Mengekstrak entri ke sistem file menggunakan jalur yang disediakan.

Ekstrak dua entri arsip ZIP, masing-masing dengan kata sandi sendiri

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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | Jalur ke file tujuan. Jika file sudah ada, akan ditimpa. |
| password | java.lang.String | Kata sandi opsional untuk dekripsi. |

**Returns:**
java.io.File - informasi file dari file yang diekstrak
### getComment() {#getComment--}
```
public final String getComment()
```


Mendapatkan komentar dari entri dalam arsip.

**Returns:**
java.lang.String - komentar entri dalam arsip
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

Dalam contoh ini event handler digunakan untuk pembatalan setelah seratus Mb pertama dari entri diekstrak.

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

Baca dari aliran untuk mendapatkan konten asli file.

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

Pengirim Event adalah sebuah instance [ArchiveEntry](../../com.aspose.zip/archiveentry).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | sebuah event yang dipicu ketika sebagian aliran mentah dikompresi |

### setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


Menetapkan sebuah peristiwa yang dipicu ketika sebagian aliran mentah diekstrak.

Dalam contoh ini event handler digunakan untuk menghitung bagian ukuran yang diproses dalam persen.

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

Pengirim Event adalah sebuah instance [ArchiveEntry](../../com.aspose.zip/archiveentry). Dimungkinkan untuk membatalkan ekstraksi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | sebuah event yang dipicu ketika sebagian aliran mentah diekstrak. |

### setModificationTime(Date value) {#setModificationTime-java.util.Date-}
```
public final void setModificationTime(Date value)
```


Menetapkan tanggal dan waktu terakhir dimodifikasi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | tanggal dan waktu terakhir diubah |

