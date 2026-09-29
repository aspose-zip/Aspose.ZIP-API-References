---
title: "GzipArchive"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Kelas ini mewakili file arsip gzip."
type: docs
weight: 69
url: /id/java/com.aspose.zip/gziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class GzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Kelas ini merepresentasikan file arsip gzip. Gunakan untuk membuat atau mengekstrak arsip gzip.

Algoritma kompresi Gzip didasarkan pada algoritma DEFLATE, yang merupakan kombinasi dari LZ77 dan pengkodean Huffman.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [GzipArchive()](#GzipArchive--) | Menginisialisasi instance baru dari kelas [GzipArchive](../../com.aspose.zip/gziparchive) yang disiapkan untuk kompresi. |
| [GzipArchive(InputStream sourceStream)](#GzipArchive-java.io.InputStream-) | Menginisialisasi instance baru dari kelas [GzipArchive](../../com.aspose.zip/gziparchive) yang disiapkan untuk dekompresi. |
| [GzipArchive(InputStream sourceStream, boolean parseHeader)](#GzipArchive-java.io.InputStream-boolean-) | Menginisialisasi instance baru dari kelas [GzipArchive](../../com.aspose.zip/gziparchive) yang disiapkan untuk dekompresi. |
| [GzipArchive(InputStream sourceStream, GzipLoadOptions options)](#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-) | Menginisialisasi instance baru dari kelas [GzipArchive](../../com.aspose.zip/gziparchive) yang disiapkan untuk dekompresi. |
| [GzipArchive(String path, GzipLoadOptions options)](#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-) | Menginisialisasi instance baru dari kelas [GzipArchive](../../com.aspose.zip/gziparchive) yang disiapkan untuk dekompresi. |
| [GzipArchive(String path)](#GzipArchive-java.lang.String-) | Menginisialisasi instance baru dari kelas [GzipArchive](../../com.aspose.zip/gziparchive). |
| [GzipArchive(String path, boolean parseHeader)](#GzipArchive-java.lang.String-boolean-) | Menginisialisasi instance baru dari kelas [GzipArchive](../../com.aspose.zip/gziparchive). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Mengekstrak arsip ke aliran yang disediakan. |
| [extract(String path)](#extract-java.lang.String-) | Mengekstrak arsip ke file berdasarkan jalur. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Mengekstrak konten arsip ke direktori yang diberikan. |
| [getFileEntries()](#getFileEntries--) | Mendapatkan entri tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip gzip. |
| [getFormat()](#getFormat--) | Mendapatkan format arsip. |
| [getLength()](#getLength--) | Mendapatkan ukuran file asli. |
| [getName()](#getName--) | Nama file asli. |
| [getUncompressedSize()](#getUncompressedSize--) | Mendapatkan ukuran file asli. |
| [open()](#open--) | Membuka arsip untuk ekstraksi dan menyediakan aliran dengan konten arsip. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Menyimpan arsip ke aliran yang disediakan. |
| [save(String destinationFileName)](#save-java.lang.String-) | Menyimpan arsip ke file tujuan yang disediakan. |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | Mengatur konten yang akan dikompresi dalam arsip. |
| [setSource(File file)](#setSource-java.io.File-) | Mengatur konten yang akan dikompresi dalam arsip. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Mengatur konten yang akan dikompresi dalam arsip. |
| [setSource(String path)](#setSource-java.lang.String-) | Mengatur konten yang akan dikompresi dalam arsip. |
### GzipArchive() {#GzipArchive--}
```
public GzipArchive()
```


Menginisialisasi instance baru dari kelas [GzipArchive](../../com.aspose.zip/gziparchive) yang disiapkan untuk kompresi.

Contoh berikut menunjukkan cara mengompresi sebuah file.

```

``````

try (GzipArchive archive = new GzipArchive())
{
archive.setSource("data.bin");
archive.save("archive.gz");
}
 
```



### GzipArchive(InputStream sourceStream) {#GzipArchive-java.io.InputStream-}
```
public GzipArchive(InputStream sourceStream)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Konstruktor ini tidak melakukan dekompresi. Lihat metode [open()](../../com.aspose.zip/gziparchive\#open--) untuk dekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Sumber arsip. |

### GzipArchive(InputStream sourceStream, boolean parseHeader) {#GzipArchive-java.io.InputStream-boolean-}
```
public GzipArchive(InputStream sourceStream, boolean parseHeader)
```


Menginisialisasi instance baru dari kelas [GzipArchive](../../com.aspose.zip/gziparchive) yang disiapkan untuk dekompresi.

Buka arsip dari aliran dan ekstrak ke `ByteArrayOutputStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### GzipArchive(InputStream sourceStream, GzipLoadOptions options) {#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(InputStream sourceStream, GzipLoadOptions options)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     GzipLoadOptions options = new GzipLoadOptions();
     try (GzipArchive archive = new GzipArchive(new FileInputStream("archive.gz"), options)) {
         archive.extract(ms);
     } catch (IOException ex) {
     }
 
```

Konstruktor ini tidak melakukan dekompresi. Lihat metode [open()](../../com.aspose.zip/gziparchive\#open--) untuk dekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Sumber arsip. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Opsi untuk memuat arsip dengan. |

### GzipArchive(String path, GzipLoadOptions options) {#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(String path, GzipLoadOptions options)
```


Menginisialisasi instance baru dari kelas [GzipArchive](../../com.aspose.zip/gziparchive) yang disiapkan untuk dekompresi.

Buka arsip dari file dengan jalur dan ekstrak ke `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
GzipLoadOptions options = new GzipLoadOptions();
try (GzipArchive archive = new GzipArchive("archive.gz", options)) {
archive.extract(ms);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Options to load the archive with. |

### GzipArchive(String path) {#GzipArchive-java.lang.String-}
```
public GzipArchive(String path)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Konstruktor ini tidak melakukan dekompresi. Lihat metode [open()](../../com.aspose.zip/gziparchive\#open--) untuk dekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | Jalur ke file arsip. |

### GzipArchive(String path, boolean parseHeader) {#GzipArchive-java.lang.String-boolean-}
```
public GzipArchive(String path, boolean parseHeader)
```


Menginisialisasi instance baru dari kelas [GzipArchive](../../com.aspose.zip/gziparchive).

Buka arsip dari file dengan jalur dan ekstrak ke `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive("archive.gz")) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

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

     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tujuan | java.io.OutputStream | Aliran tujuan. Harus dapat ditulis. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Mengekstrak arsip ke file berdasarkan jalur.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | Jalur ke file tujuan. Jika file sudah ada, akan ditimpa. |

**Returns:**
java.io.File - informasi file dari file yang diekstrak
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Mengekstrak konten arsip ke direktori yang diberikan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | Jalur ke direktori tempat menempatkan file yang diekstrak. |

Jika direktori tidak ada, itu akan dibuat. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Mendapatkan entri tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip gzip.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entri dari tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip gzip.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Mendapatkan format arsip.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


Mendapatkan ukuran file asli.

Selama dekompresi, properti ini mungkin berisi ukuran yang tidak tepat. Jika ukuran file yang tidak terkompresi melebihi 4GB, properti ini akan memberikan nilai yang salah karena batas 32-bit pada header.

**Returns:**
java.lang.Long - ukuran file asli
### getName() {#getName--}
```
public final String getName()
```


Nama file asli.

**Returns:**
java.lang.String - nama file asli
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Mendapatkan ukuran file asli.

Selama dekompresi, properti ini mungkin berisi ukuran yang tidak tepat. Jika ukuran file yang tidak terkompresi melebihi 4GB, properti ini akan memberikan nilai yang salah karena batas 32-bit pada header.

**Returns:**
long - ukuran file asli.
### open() {#open--}
```
public final InputStream open()
```


Membuka arsip untuk ekstraksi dan menyediakan aliran dengan konten arsip.

Mengekstrak arsip dan menyalin konten yang diekstrak ke aliran file.

```

``````

try (GzipArchive archive = new GzipArchive("archive.gz")) {
try (FileOutputStream extracted = new FileOutputStream(\"data.bin\")) {
InputStream unpacked = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - The stream that represents the contents of the archive.
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Writes compressed data to http response stream.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(httpResponseStream);
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | outputStream | java.io.OutputStream | Aliran tujuan. |

`outputStream` harus dapat ditulis. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Menyimpan arsip ke file tujuan yang disediakan.

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource("data.bin");
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### setSource(TarArchive tarArchive) {#setSource-com.aspose.zip.TarArchive-}
```
public final void setSource(TarArchive tarArchive)
```


Sets the content to be compressed within the archive.

```

``````

     try (TarArchive tarArchive = new TarArchive()) {
         tarArchive.createEntry("first.bin", "data1.bin");
         tarArchive.createEntry("second.bin", "data2.bin");
         try (GzipArchive gzippedArchive = new GzipArchive()) {
             gzippedArchive.setSource(tarArchive);
             gzippedArchive.save("archive.tar.gz");
         }
     }
 
```

Gunakan metode ini untuk menyusun arsip tar.gz gabungan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | Arsip Tar yang akan dikompresi. |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Mengatur konten yang akan dikompresi dalam arsip.

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | The reference to a file to be compressed. |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.gz");
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | java.io.InputStream | Aliran masukan untuk arsip. |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Mengatur konten yang akan dikompresi dalam arsip.

Buka arsip dari file dengan jalur dan ekstrak ke `MemoryStream`

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource("data.bin");
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file to be compressed. |

