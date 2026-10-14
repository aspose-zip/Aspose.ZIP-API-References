---
title: "IsoArchive"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Mewakili arsip ISO ISO 9660."
type: docs
weight: 71
url: /id/java/com.aspose.zip/isoarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public final class IsoArchive implements IArchive, AutoCloseable
```

Mewakili arsip ISO (ISO 9660).
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [IsoArchive()](#IsoArchive--) | Menginisialisasi instance baru dari kelas [IsoArchive](../../com.aspose.zip/isoarchive) dan membuat arsip ISO kosong untuk menambahkan file dan direktori baru. |
| [IsoArchive(InputStream sourceStream)](#IsoArchive-java.io.InputStream-) | Menginisialisasi instance baru dari kelas [IsoArchive](../../com.aspose.zip/isoarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)](#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-) | Menginisialisasi instance baru dari kelas [IsoArchive](../../com.aspose.zip/isoarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [IsoArchive(String path)](#IsoArchive-java.lang.String-) | Menginisialisasi instance baru dari kelas [IsoArchive](../../com.aspose.zip/isoarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [IsoArchive(String path, IsoLoadOptions loadOptions)](#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-) | Menginisialisasi instance baru dari kelas [IsoArchive](../../com.aspose.zip/isoarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createDirectory(String name)](#createDirectory-java.lang.String-) | Menambahkan direktori ke gambar ISO. |
| [createEntry(String name)](#createEntry-java.lang.String-) | Menambahkan file ke gambar ISO. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Menambahkan file ke gambar ISO. |
| [createEntry(String name, String filePath)](#createEntry-java.lang.String-java.lang.String-) | Menambahkan file ke gambar ISO. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Mengekstrak semua entri ke direktori yang ditentukan. |
| [getEntries()](#getEntries--) | Mendapatkan entri tipe [IsoEntry](../../com.aspose.zip/isoentry) yang membentuk arsip. |
| [getFileEntries()](#getFileEntries--) | Mendapatkan entri tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip. |
| [getFormat()](#getFormat--) | Mendapatkan format arsip. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Menyimpan gambar ISO ke aliran yang ditentukan. |
| [save(OutputStream stream, IsoSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-) | Menyimpan gambar ISO ke aliran yang ditentukan. |
| [save(String path)](#save-java.lang.String-) | Menyimpan gambar ISO ke jalur yang ditentukan. |
| [save(String path, IsoSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.IsoSaveOptions-) | Menyimpan gambar ISO ke jalur yang ditentukan. |
### IsoArchive() {#IsoArchive--}
```
public IsoArchive()
```


Menginisialisasi instance baru dari kelas [IsoArchive](../../com.aspose.zip/isoarchive) dan membuat arsip ISO kosong untuk menambahkan file dan direktori baru.

Contoh berikut menunjukkan cara membuat arsip ISO kosong baru dan menambahkan file ke dalamnya:

```

``````

// Membuat arsip ISO kosong baru
try (IsoArchive isoArchive = new IsoArchive()) {
// Menambahkan file ke arsip ISO
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// Menyimpan arsip ISO ke file
isoArchive.save("new_archive.iso");
}
 
```



### IsoArchive(InputStream sourceStream) {#IsoArchive-java.io.InputStream-}
```
public IsoArchive(InputStream sourceStream)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Konstruktor ini tidak mengekstrak entri apa pun.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | java.io.InputStream | sumber arsip |

### IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions) {#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)
```


Menginisialisasi instance baru dari kelas [IsoArchive](../../com.aspose.zip/isoarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip.

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori.

```

``````

try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### IsoArchive(String path) {#IsoArchive-java.lang.String-}
```
public IsoArchive(String path)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive("archive.iso")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

Konstruktor ini tidak mengekstrak entri apa pun.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur ke file arsip |

### IsoArchive(String path, IsoLoadOptions loadOptions) {#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(String path, IsoLoadOptions loadOptions)
```


Menginisialisasi instance baru dari kelas [IsoArchive](../../com.aspose.zip/isoarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip.

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori.

```

``````

try (IsoArchive archive = new IsoArchive(\"archive.iso\")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### close() {#close--}
```
public void close()
```




### createDirectory(String name) {#createDirectory-java.lang.String-}
```
public final IsoEntry createDirectory(String name)
```


Adds a directory to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the directory in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name) {#createEntry-java.lang.String-}
```
public final IsoEntry createEntry(String name)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final IsoEntry createEntry(String name, InputStream source)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| source | java.io.InputStream | the stream containing the file data |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, String filePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final IsoEntry createEntry(String name, String filePath)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| filePath | java.lang.String | the path of the file |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all entries to the specified directory.

The following example shows how to extract all entries to a directory:

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationDirectory | java.lang.String | direktori untuk mengekstrak entri |

### getEntries() {#getEntries--}
```
public final List<IsoEntry> getEntries()
```


Mendapatkan entri tipe [IsoEntry](../../com.aspose.zip/isoentry) yang membentuk arsip.

**Returns:**
java.util.List&lt;com.aspose.zip.IsoEntry&gt; - entri dari tipe [IsoEntry](../../com.aspose.zip/isoentry) yang membentuk arsip iso
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Mendapatkan entri tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entri dari tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip iso
### getFormat() {#getFormat--}
```
public ArchiveFormat getFormat()
```


Mendapatkan format arsip.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream stream)
```


Menyimpan gambar ISO ke aliran yang ditentukan.

Contoh berikut menunjukkan cara menyimpan arsip ISO ke aliran memori:

```

``````

ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
// Membuat arsip ISO kosong baru
try (IsoArchive isoArchive = new IsoArchive()) {
// Menambahkan file ke arsip ISO
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// Simpan arsip ISO ke aliran memori
isoArchive.save(memoryStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the stream where the ISO image will be saved |

### save(OutputStream stream, IsoSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-}
```
public final void save(OutputStream stream, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified stream.

The following example shows how to save an ISO archive to a memory stream:

```

``````

     ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a memory stream
         isoArchive.save(memoryStream);
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.OutputStream | aliran tempat gambar ISO akan disimpan |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | opsi untuk menyimpan arsip ISO |

### save(String path) {#save-java.lang.String-}
```
public final void save(String path)
```


Menyimpan gambar ISO ke jalur yang ditentukan.

Contoh berikut menunjukkan cara menyimpan arsip ISO ke file:

```

``````

// Membuat arsip ISO kosong baru
try (IsoArchive isoArchive = new IsoArchive()) {
// Menambahkan file ke arsip ISO
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// Menyimpan arsip ISO ke file
isoArchive.save("new_archive.iso");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path where the ISO image will be saved |

### save(String path, IsoSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.IsoSaveOptions-}
```
public final void save(String path, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified path.

The following example shows how to save an ISO archive to a file:

```

``````

     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a file
         isoArchive.save("new_archive.iso");
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur tempat gambar ISO akan disimpan |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | opsi untuk menyimpan arsip ISO |

