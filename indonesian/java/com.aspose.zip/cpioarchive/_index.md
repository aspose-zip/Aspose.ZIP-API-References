---
title: "CpioArchive"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Kelas ini mewakili file arsip cpio."
type: docs
weight: 57
url: /id/java/com.aspose.zip/cpioarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class CpioArchive implements IArchive, AutoCloseable
```

Kelas ini mewakili file arsip cpio.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [CpioArchive()](#CpioArchive--) | Menginisialisasi sebuah instance baru dari kelas [CpioArchive](../../com.aspose.zip/cpioarchive). |
| [CpioArchive(InputStream sourceStream)](#CpioArchive-java.io.InputStream-) | Menginisialisasi sebuah instance baru dari kelas [CpioArchive](../../com.aspose.zip/cpioarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [CpioArchive(String path)](#CpioArchive-java.lang.String-) | Menginisialisasi sebuah instance baru dari kelas [CpioArchive](../../com.aspose.zip/cpioarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Membuat satu entri dalam arsip. |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Membuat satu entri dalam arsip. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Membuat satu entri dalam arsip. |
| [createEntry(String name, String sourcePath)](#createEntry-java.lang.String-java.lang.String-) | Membuat satu entri dalam arsip. |
| [createEntry(String name, String sourcePath, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Membuat satu entri dalam arsip. |
| [deleteEntry(CpioEntry entry)](#deleteEntry-com.aspose.zip.CpioEntry-) | Menghapus kemunculan pertama dari entri tertentu dari daftar entri. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Menghapus entri dari daftar entri berdasarkan indeks. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Mengekstrak semua file dalam arsip ke direktori yang disediakan. |
| [getEntries()](#getEntries--) | Mendapatkan entri berjenis [CpioEntry](../../com.aspose.zip/cpioentry) yang membentuk arsip cpio. |
| [getFileEntries()](#getFileEntries--) | Mendapatkan entri dari tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip cpio. |
| [getFormat()](#getFormat--) | Mendapatkan format arsip. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Menyimpan arsip ke aliran yang disediakan. |
| [save(OutputStream output, CpioFormat cpioFormat)](#save-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Menyimpan arsip ke aliran yang disediakan. |
| [save(String destinationFileName)](#save-java.lang.String-) | Menyimpan arsip ke file tujuan yang disediakan. |
| [save(String destinationFileName, CpioFormat cpioFormat)](#save-java.lang.String-com.aspose.zip.CpioFormat-) | Menyimpan arsip ke file tujuan yang disediakan. |
| [saveGzipped(OutputStream output)](#saveGzipped-java.io.OutputStream-) | Menyimpan arsip ke aliran dengan kompresi gzip. |
| [saveGzipped(OutputStream output, CpioFormat cpioFormat)](#saveGzipped-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Menyimpan arsip ke aliran dengan kompresi gzip. |
| [saveGzipped(String path)](#saveGzipped-java.lang.String-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi gzip. |
| [saveGzipped(String path, CpioFormat cpioFormat)](#saveGzipped-java.lang.String-com.aspose.zip.CpioFormat-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi gzip. |
| [saveLZMACompressed(OutputStream output)](#saveLZMACompressed-java.io.OutputStream-) | Menyimpan arsip ke aliran dengan kompresi LZMA. |
| [saveLZMACompressed(OutputStream output, CpioFormat cpioFormat)](#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Menyimpan arsip ke aliran dengan kompresi LZMA. |
| [saveLZMACompressed(String path)](#saveLZMACompressed-java.lang.String-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi lzma. |
| [saveLZMACompressed(String path, CpioFormat cpioFormat)](#saveLZMACompressed-java.lang.String-com.aspose.zip.CpioFormat-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi lzma. |
| [saveLzipped(OutputStream output)](#saveLzipped-java.io.OutputStream-) | Menyimpan arsip ke aliran dengan kompresi lzip. |
| [saveLzipped(OutputStream output, CpioFormat cpioFormat)](#saveLzipped-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Menyimpan arsip ke aliran dengan kompresi lzip. |
| [saveLzipped(String path)](#saveLzipped-java.lang.String-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi lzip. |
| [saveLzipped(String path, CpioFormat cpioFormat)](#saveLzipped-java.lang.String-com.aspose.zip.CpioFormat-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi lzip. |
| [saveXzCompressed(OutputStream output)](#saveXzCompressed-java.io.OutputStream-) | Menyimpan arsip ke aliran dengan kompresi xz. |
| [saveXzCompressed(OutputStream output, CpioFormat cpioFormat)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Menyimpan arsip ke aliran dengan kompresi xz. |
| [saveXzCompressed(OutputStream output, CpioFormat cpioFormat, XzArchiveSettings settings)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-com.aspose.zip.XzArchiveSettings-) | Menyimpan arsip ke aliran dengan kompresi xz. |
| [saveXzCompressed(String path)](#saveXzCompressed-java.lang.String-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi xz. |
| [saveXzCompressed(String path, CpioFormat cpioFormat)](#saveXzCompressed-java.lang.String-com.aspose.zip.CpioFormat-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi xz. |
| [saveXzCompressed(String path, CpioFormat cpioFormat, XzArchiveSettings settings)](#saveXzCompressed-java.lang.String-com.aspose.zip.CpioFormat-com.aspose.zip.XzArchiveSettings-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi xz. |
| [saveZCompressed(OutputStream output)](#saveZCompressed-java.io.OutputStream-) | Menyimpan arsip ke aliran dengan kompresi Z. |
| [saveZCompressed(OutputStream output, CpioFormat cpioFormat)](#saveZCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Menyimpan arsip ke aliran dengan kompresi Z. |
| [saveZCompressed(String path)](#saveZCompressed-java.lang.String-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi Z. |
| [saveZCompressed(String path, CpioFormat cpioFormat)](#saveZCompressed-java.lang.String-com.aspose.zip.CpioFormat-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi Z. |
| [saveZstandard(OutputStream output)](#saveZstandard-java.io.OutputStream-) | Menyimpan arsip ke aliran dengan kompresi Zstandard. |
| [saveZstandard(OutputStream output, CpioFormat cpioFormat)](#saveZstandard-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Menyimpan arsip ke aliran dengan kompresi Zstandard. |
| [saveZstandard(String path)](#saveZstandard-java.lang.String-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi Zstandard. |
| [saveZstandard(String path, CpioFormat cpioFormat)](#saveZstandard-java.lang.String-com.aspose.zip.CpioFormat-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi Zstandard. |
### CpioArchive() {#CpioArchive--}
```
public CpioArchive()
```


Menginisialisasi sebuah instance baru dari kelas [CpioArchive](../../com.aspose.zip/cpioarchive).

Contoh berikut menunjukkan cara mengompresi sebuah file.

```

``````

try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.cpio");
}
 
```



### CpioArchive(InputStream sourceStream) {#CpioArchive-java.io.InputStream-}
```
public CpioArchive(InputStream sourceStream)
```


Initializes a new instance of the [CpioArchive](../../com.aspose.zip/cpioarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (CpioArchive archive = new CpioArchive(new FileInputStream("archive.cpio"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Konstruktor ini tidak mengekstrak entri apa pun. Lihat metode [CpioEntry.open()](../../com.aspose.zip/cpioentry\#open--) untuk mengekstrak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | java.io.InputStream | sumber arsip |

### CpioArchive(String path) {#CpioArchive-java.lang.String-}
```
public CpioArchive(String path)
```


Menginisialisasi sebuah instance baru dari kelas [CpioArchive](../../com.aspose.zip/cpioarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip.

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori.

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [CpioEntry.open()](../../com.aspose.zip/cpioentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final CpioArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(cpioFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| direktori | java.io.File | direktori untuk dikompresi |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final CpioArchive createEntries(File directory, boolean includeRootDirectory)
```


Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan.

```

``````

try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(cpioFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final CpioArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(cpioFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceDirectory | java.lang.String | direktori untuk dikompresi |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final CpioArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan.

```

``````

try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(cpioFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final CpioEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     java.io.File file = new File("data.bin");
     try (CpioArchive archive = new CpioArchive()) {
         archive.createEntry("test.bin", file);
         archive.save("archive.cpio");
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String | nama entri |
| file | java.io.File | metadata file atau folder yang akan dikompresi |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final CpioEntry createEntry(String name, File file, boolean openImmediately)
```


Membuat satu entri dalam arsip.

```

``````

java.io.File file = new File("data.bin");
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("test.bin", file);
archive.save("archive.cpio");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final CpioEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (CpioArchive archive = new CpioArchive()) {
         archive.createEntry("data.bin", new FileInputStream("data.bin"));
         archive.save("archive.cpio");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String | nama entri |
| source | java.io.InputStream | stream input untuk entri tersebut |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### createEntry(String name, String sourcePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final CpioEntry createEntry(String name, String sourcePath)
```


Membuat satu entri dalam arsip.

```

``````

try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.cpio");
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `sourcePath` parameter does not affect the entry name

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| sourcePath | java.lang.String | path to file to be compressed. |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### createEntry(String name, String sourcePath, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final CpioEntry createEntry(String name, String sourcePath, boolean openImmediately)
```


Creates a single entry within the archive.

```

``````

     try (CpioArchive archive = new CpioArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.cpio");
     }
 
```

Nama entri hanya diatur dalam parameter `name`. Nama file yang diberikan dalam parameter `sourcePath` tidak memengaruhi nama entri

Jika file dibuka segera dengan parameter `openImmediately`, file akan diblokir hingga arsip dibuang

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String | nama entri |
| sourcePath | java.lang.String | jalur ke file yang akan dikompresi. |
| openImmediately | boolean | true, jika membuka file segera, jika tidak membuka file saat menyimpan arsip. |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### deleteEntry(CpioEntry entry) {#deleteEntry-com.aspose.zip.CpioEntry-}
```
public final CpioArchive deleteEntry(CpioEntry entry)
```


Menghapus kemunculan pertama dari entri tertentu dari daftar entri.

Berikut cara menghapus semua entri kecuali yang terakhir:

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
while (archive.getEntries().size() > 1)
archive.deleteEntry(archive.getEntries().get(0));
archive.save("outputCpioFile.cpio");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [CpioEntry](../../com.aspose.zip/cpioentry) | the entry to remove from the entries list |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final CpioArchive deleteEntry(int entryIndex)
```


Removes the entry from the entry list by index.

```

``````

     try (CpioArchive archive = new CpioArchive("two_files.cpio")) {
         archive.deleteEntry(0);
         archive.save("single_file.cpio");
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| entryIndex | int | indeks berbasis nol dari entri yang akan dihapus |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - the archive with the entry deleted
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Mengekstrak semua file dalam arsip ke direktori yang disediakan.

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getEntries() {#getEntries--}
```
public final List<CpioEntry> getEntries()
```


Gets entries of [CpioEntry](../../com.aspose.zip/cpioentry) type constituting the cpio archive.

**Returns:**
java.util.List&lt;com.aspose.zip.CpioEntry&gt; - entries of [CpioEntry](../../com.aspose.zip/cpioentry) type constituting the cpio archive.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the cpio archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the cpio archive.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves archive to the stream provided.

```

``````

     try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry1", "data.bin");
             archive.save(cpioFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | output | java.io.OutputStream | stream tujuan. |

`output` harus dapat ditulis |

### save(OutputStream output, CpioFormat cpioFormat) {#save-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void save(OutputStream output, CpioFormat cpioFormat)
```


Menyimpan arsip ke aliran yang disediakan.

```

``````

try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(cpioFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

```

``````

     try (CpioArchive archive = new CpioArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("archive.cpio");
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | destinationFileName | java.lang.String | jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa. |

Dimungkinkan menyimpan arsip ke jalur yang sama dari mana ia dimuat. Namun, ini tidak disarankan karena pendekatan ini menggunakan penyalinan ke file sementara |

### save(String destinationFileName, CpioFormat cpioFormat) {#save-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void save(String destinationFileName, CpioFormat cpioFormat)
```


Menyimpan arsip ke file tujuan yang disediakan.

```

``````

try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save("archive.cpio");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten.

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveGzipped(OutputStream output) {#saveGzipped-java.io.OutputStream-}
```
public final void saveGzipped(OutputStream output)
```


Saves archive to the stream with gzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.gz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveGzipped(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | output | java.io.OutputStream | stream tujuan. |

`output` harus dapat ditulis |

### saveGzipped(OutputStream output, CpioFormat cpioFormat) {#saveGzipped-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveGzipped(OutputStream output, CpioFormat cpioFormat)
```


Menyimpan arsip ke aliran dengan kompresi gzip.

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.gz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveGzipped(String path) {#saveGzipped-java.lang.String-}
```
public final void saveGzipped(String path)
```


Saves archive to the file by path with gzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveGzipped("result.cpio.gz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa |

### saveGzipped(String path, CpioFormat cpioFormat) {#saveGzipped-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveGzipped(String path, CpioFormat cpioFormat)
```


Menyimpan arsip ke file berdasarkan jalur dengan kompresi gzip.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped("result.cpio.gz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveLZMACompressed(OutputStream output) {#saveLZMACompressed-java.io.OutputStream-}
```
public final void saveLZMACompressed(OutputStream output)
```


Saves the archive to the stream with LZMA compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.lzma")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZMACompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```

Penting: arsip cpio dibuat kemudian dikompresi dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | output | java.io.OutputStream | stream tujuan. |

`output` harus dapat ditulis |

### saveLZMACompressed(OutputStream output, CpioFormat cpioFormat) {#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveLZMACompressed(OutputStream output, CpioFormat cpioFormat)
```


Menyimpan arsip ke aliran dengan kompresi LZMA.

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.lzma")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed(result);
}
}
} catch (IOException ex) {
}
 
```

Important: cpio archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveLZMACompressed(String path) {#saveLZMACompressed-java.lang.String-}
```
public final void saveLZMACompressed(String path)
```


Saves the archive to the file by path with lzma compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZMACompressed("result.cpio.lzma");
         }
     } catch (IOException ex) {
     }
 
```

Penting: arsip cpio dibuat kemudian dikompresi dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa |

### saveLZMACompressed(String path, CpioFormat cpioFormat) {#saveLZMACompressed-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveLZMACompressed(String path, CpioFormat cpioFormat)
```


Menyimpan arsip ke file berdasarkan jalur dengan kompresi lzma.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed("result.cpio.lzma");
}
} catch (IOException ex) {
}
 
```

Important: cpio archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveLzipped(OutputStream output) {#saveLzipped-java.io.OutputStream-}
```
public final void saveLzipped(OutputStream output)
```


Saves archive to the stream with lzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.lz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLzipped(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | output | java.io.OutputStream | stream tujuan. |

`output` harus dapat ditulis |

### saveLzipped(OutputStream output, CpioFormat cpioFormat) {#saveLzipped-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveLzipped(OutputStream output, CpioFormat cpioFormat)
```


Menyimpan arsip ke aliran dengan kompresi lzip.

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.lz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveLzipped(String path) {#saveLzipped-java.lang.String-}
```
public final void saveLzipped(String path)
```


Saves archive to the file by path with lzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLzipped("result.cpio.lz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa |

### saveLzipped(String path, CpioFormat cpioFormat) {#saveLzipped-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveLzipped(String path, CpioFormat cpioFormat)
```


Menyimpan arsip ke file berdasarkan jalur dengan kompresi lzip.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped("result.cpio.lz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveXzCompressed(OutputStream output) {#saveXzCompressed-java.io.OutputStream-}
```
public final void saveXzCompressed(OutputStream output)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveXzCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | output | java.io.OutputStream | stream tujuan. |

`output`Aliran harus dapat ditulis |

### saveXzCompressed(OutputStream output, CpioFormat cpioFormat) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveXzCompressed(OutputStream output, CpioFormat cpioFormat)
```


Menyimpan arsip ke aliran dengan kompresi xz.

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output`The stream must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveXzCompressed(OutputStream output, CpioFormat cpioFormat, XzArchiveSettings settings) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(OutputStream output, CpioFormat cpioFormat, XzArchiveSettings settings)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveXzCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | output | java.io.OutputStream | stream tujuan. |

`output`Aliran harus dapat ditulis. |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | mendefinisikan format header cpio |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | sekumpulan pengaturan khusus arsip xz: ukuran kamus, ukuran blok, tipe pemeriksaan |

### saveXzCompressed(String path) {#saveXzCompressed-java.lang.String-}
```
public final void saveXzCompressed(String path)
```


Menyimpan arsip ke file berdasarkan jalur dengan kompresi xz.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed("result.cpio.xz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveXzCompressed(String path, CpioFormat cpioFormat) {#saveXzCompressed-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveXzCompressed(String path, CpioFormat cpioFormat)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.cpio.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | mendefinisikan format header cpio |

### saveXzCompressed(String path, CpioFormat cpioFormat, XzArchiveSettings settings) {#saveXzCompressed-java.lang.String-com.aspose.zip.CpioFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(String path, CpioFormat cpioFormat, XzArchiveSettings settings)
```


Menyimpan arsip ke file berdasarkan jalur dengan kompresi xz.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed("result.cpio.xz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | set of setting particular xz archive: dictionary size, block size, check type |

### saveZCompressed(OutputStream output) {#saveZCompressed-java.io.OutputStream-}
```
public final void saveZCompressed(OutputStream output)
```


Saves archive to the stream with Z compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.Z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | output | java.io.OutputStream | stream tujuan. |

`output` harus dapat ditulis |

### saveZCompressed(OutputStream output, CpioFormat cpioFormat) {#saveZCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveZCompressed(OutputStream output, CpioFormat cpioFormat)
```


Menyimpan arsip ke aliran dengan kompresi Z.

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.Z")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveZCompressed(String path) {#saveZCompressed-java.lang.String-}
```
public final void saveZCompressed(String path)
```


Saves archive to the file by path with Z compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZCompressed("result.cpio.Z");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa |

### saveZCompressed(String path, CpioFormat cpioFormat) {#saveZCompressed-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveZCompressed(String path, CpioFormat cpioFormat)
```


Menyimpan arsip ke file berdasarkan jalur dengan kompresi Z.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed("result.cpio.Z");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | d cpio header format |

### saveZstandard(OutputStream output) {#saveZstandard-java.io.OutputStream-}
```
public final void saveZstandard(OutputStream output)
```


Saves archive to the stream with Zstandard compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.zst")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZstandard(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | output | java.io.OutputStream | stream tujuan. |

`output` harus dapat ditulis |

### saveZstandard(OutputStream output, CpioFormat cpioFormat) {#saveZstandard-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveZstandard(OutputStream output, CpioFormat cpioFormat)
```


Menyimpan arsip ke aliran dengan kompresi Zstandard.

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.zst")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveZstandard(String path) {#saveZstandard-java.lang.String-}
```
public final void saveZstandard(String path)
```


Saves archive to the file by path with Zstandard compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZstandard("result.cpio.zst");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa |

### saveZstandard(String path, CpioFormat cpioFormat) {#saveZstandard-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveZstandard(String path, CpioFormat cpioFormat)
```


Menyimpan arsip ke file berdasarkan jalur dengan kompresi Zstandard.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard("result.cpio.zst");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

