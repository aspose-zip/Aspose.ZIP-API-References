---
title: "TarArchive"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Kelas ini mewakili file arsip tar."
type: docs
weight: 125
url: /id/java/com.aspose.zip/tararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class TarArchive implements IArchive, AutoCloseable
```

Kelas ini mewakili file arsip tar. Gunakan untuk menyusun, mengekstrak, atau memperbarui arsip tar.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [TarArchive()](#TarArchive--) | Menginisialisasi instance baru dari kelas [TarArchive](../../com.aspose.zip/tararchive). |
| [TarArchive(InputStream sourceStream)](#TarArchive-java.io.InputStream-) | Menginisialisasi instance baru dari kelas [Archive](../../com.aspose.zip/archive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [TarArchive(String path)](#TarArchive-java.lang.String-) | Menginisialisasi instance baru dari kelas [TarArchive](../../com.aspose.zip/tararchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
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
| [createEntry(String name, InputStream source, File file)](#createEntry-java.lang.String-java.io.InputStream-java.io.File-) | Membuat satu entri dalam arsip. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Membuat satu entri dalam arsip. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Membuat satu entri dalam arsip. |
| [deleteEntry(TarEntry entry)](#deleteEntry-com.aspose.zip.TarEntry-) | Menghapus kemunculan pertama dari entri tertentu dari daftar entri. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Menghapus entri dari daftar entri berdasarkan indeks. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Mengekstrak semua file dalam arsip ke direktori yang disediakan. |
| [fromGZip(InputStream source)](#fromGZip-java.io.InputStream-) | Mengekstrak arsip gzip yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak. |
| [fromGZip(String path)](#fromGZip-java.lang.String-) | Mengekstrak arsip gzip yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak. |
| [fromLZ4(InputStream source)](#fromLZ4-java.io.InputStream-) | Mengekstrak arsip LZ4 yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak. |
| [fromLZ4(String path)](#fromLZ4-java.lang.String-) | Mengekstrak arsip LZ4 yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak. |
| [fromLZMA(InputStream source)](#fromLZMA-java.io.InputStream-) | Mengekstrak arsip LZMA yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak. |
| [fromLZMA(String path)](#fromLZMA-java.lang.String-) | Mengekstrak arsip LZMA yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak. |
| [fromLZip(InputStream source)](#fromLZip-java.io.InputStream-) | Mengekstrak arsip lzip yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak. |
| [fromLZip(String path)](#fromLZip-java.lang.String-) | Mengekstrak arsip lzip yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak. |
| [fromXz(InputStream source)](#fromXz-java.io.InputStream-) | Mengekstrak arsip format xz yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak. |
| [fromXz(String path)](#fromXz-java.lang.String-) | Mengekstrak arsip format xz yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak. |
| [fromZ(InputStream source)](#fromZ-java.io.InputStream-) | Mengekstrak arsip format Z yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak. |
| [fromZ(String path)](#fromZ-java.lang.String-) | Mengekstrak arsip format Z yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak. |
| [fromZstandard(InputStream source)](#fromZstandard-java.io.InputStream-) | Mengekstrak arsip Zstandard yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak. |
| [fromZstandard(String path)](#fromZstandard-java.lang.String-) | Mengekstrak arsip Zstandard yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak. |
| [getEntries()](#getEntries--) | Mendapatkan entri tipe [TarEntry](../../com.aspose.zip/tarentry) yang membentuk arsip. |
| [getFileEntries()](#getFileEntries--) | Mendapatkan entri tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip tar. |
| [getFormat()](#getFormat--) | Mendapatkan format arsip. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Menyimpan arsip ke aliran yang disediakan. |
| [save(OutputStream output, TarFormat format)](#save-java.io.OutputStream-com.aspose.zip.TarFormat-) | Menyimpan arsip ke aliran yang disediakan. |
| [save(String destinationFileName)](#save-java.lang.String-) | Menyimpan arsip ke file tujuan yang disediakan. |
| [save(String destinationFileName, TarFormat format)](#save-java.lang.String-com.aspose.zip.TarFormat-) | Menyimpan arsip ke file tujuan yang disediakan. |
| [saveGzipped(OutputStream output)](#saveGzipped-java.io.OutputStream-) | Menyimpan arsip ke aliran dengan kompresi gzip. |
| [saveGzipped(OutputStream output, TarFormat format)](#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | Menyimpan arsip ke aliran dengan kompresi gzip. |
| [saveGzipped(String path)](#saveGzipped-java.lang.String-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi gzip. |
| [saveGzipped(String path, TarFormat format)](#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi gzip. |
| [saveLZ4Compressed(OutputStream output)](#saveLZ4Compressed-java.io.OutputStream-) | Menyimpan arsip ke aliran dengan kompresi LZ4. |
| [saveLZ4Compressed(OutputStream output, TarFormat format)](#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Menyimpan arsip ke aliran dengan kompresi LZ4. |
| [saveLZ4Compressed(String path)](#saveLZ4Compressed-java.lang.String-) | Menyimpan arsip ke file dengan jalur menggunakan kompresi LZ4. |
| [saveLZ4Compressed(String path, TarFormat format)](#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-) | Menyimpan arsip ke file dengan jalur menggunakan kompresi LZ4. |
| [saveLZMACompressed(OutputStream output)](#saveLZMACompressed-java.io.OutputStream-) | Menyimpan arsip ke aliran dengan kompresi LZMA. |
| [saveLZMACompressed(OutputStream output, TarFormat format)](#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Menyimpan arsip ke aliran dengan kompresi LZMA. |
| [saveLZMACompressed(String path)](#saveLZMACompressed-java.lang.String-) | Menyimpan arsip ke file dengan jalur menggunakan kompresi lzma. |
| [saveLZMACompressed(String path, TarFormat format)](#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-) | Menyimpan arsip ke file dengan jalur menggunakan kompresi lzma. |
| [saveLzipped(OutputStream output)](#saveLzipped-java.io.OutputStream-) | Menyimpan arsip ke aliran dengan kompresi lzip. |
| [saveLzipped(OutputStream output, TarFormat format)](#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | Menyimpan arsip ke aliran dengan kompresi lzip. |
| [saveLzipped(String path)](#saveLzipped-java.lang.String-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi lzip. |
| [saveLzipped(String path, TarFormat format)](#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi lzip. |
| [saveXzCompressed(OutputStream output)](#saveXzCompressed-java.io.OutputStream-) | Menyimpan arsip ke aliran dengan kompresi xz. |
| [saveXzCompressed(OutputStream output, TarFormat format)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Menyimpan arsip ke aliran dengan kompresi xz. |
| [saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | Menyimpan arsip ke aliran dengan kompresi xz. |
| [saveXzCompressed(String path)](#saveXzCompressed-java.lang.String-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi xz. |
| [saveXzCompressed(String path, TarFormat format)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi xz. |
| [saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi xz. |
| [saveZCompressed(OutputStream output)](#saveZCompressed-java.io.OutputStream-) | Menyimpan arsip ke aliran dengan kompresi Z. |
| [saveZCompressed(OutputStream output, TarFormat format)](#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Menyimpan arsip ke aliran dengan kompresi Z. |
| [saveZCompressed(String path)](#saveZCompressed-java.lang.String-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi Z. |
| [saveZCompressed(String path, TarFormat format)](#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi Z. |
| [saveZstandard(OutputStream output)](#saveZstandard-java.io.OutputStream-) | Menyimpan arsip ke aliran dengan kompresi Zstandard. |
| [saveZstandard(OutputStream output, TarFormat format)](#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-) | Menyimpan arsip ke aliran dengan kompresi Zstandard. |
| [saveZstandard(String path)](#saveZstandard-java.lang.String-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi Zstandard. |
| [saveZstandard(String path, TarFormat format)](#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi Zstandard. |
### TarArchive() {#TarArchive--}
```
public TarArchive()
```


Menginisialisasi instance baru dari kelas [TarArchive](../../com.aspose.zip/tararchive).

Contoh berikut menunjukkan cara mengompresi sebuah file.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, "data.bin");
archive.save("archive.tar");
}
 
```



### TarArchive(InputStream sourceStream) {#TarArchive-java.io.InputStream-}
```
public TarArchive(InputStream sourceStream)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (TarArchive archive = new TarArchive(new FileInputStream("archive.tar"))) {
             archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Konstruktor ini tidak mengekstrak entri apa pun. Lihat metode [TarEntry.open()](../../com.aspose.zip/tarentry\#open--) untuk mengekstrak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | java.io.InputStream | sumber arsip |

### TarArchive(String path) {#TarArchive-java.lang.String-}
```
public TarArchive(String path)
```


Menginisialisasi instance baru dari kelas [TarArchive](../../com.aspose.zip/tararchive) dan menyusun daftar entri yang dapat diekstrak dari arsip.

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori.

```

``````

try (TarArchive archive = new TarArchive("archive.tar")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [TarEntry.open()](../../com.aspose.zip/tarentry\#open--) method for unpacking.

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
public final TarArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| direktori | java.io.File | direktori untuk dikompresi |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final TarArchive createEntries(File directory, boolean includeRootDirectory)
```


Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan.

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final TarArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceDirectory | java.lang.String | direktori untuk dikompresi |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final TarArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan.

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final TarEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     File fi = new File("data.bin");
     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("data.bin", fi);
         archive.save(tarFile);
     }
 
```

Nama entri hanya ditetapkan dalam parameter `name`. Nama file yang diberikan dalam parameter `file` tidak memengaruhi nama entri.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String | nama entri |
| file | java.io.File | metadata file atau folder yang akan dikompresi |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final TarEntry createEntry(String name, File file, boolean openImmediately)
```


Membuat satu entri dalam arsip.

```

``````

File fi = new File("data.bin");
try (TarArchive archive = new TarArchive()) {
archive.createEntry("data.bin", fi);
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final TarEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("bytes", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
         archive.save(tarFile);
     }
 
```

Nama entri hanya ditetapkan dalam parameter `name`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String | nama entri |
| source | java.io.InputStream | stream input untuk entri tersebut |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source, File file) {#createEntry-java.lang.String-java.io.InputStream-java.io.File-}
```
public final TarEntry createEntry(String name, InputStream source, File file)
```


Membuat satu entri dalam arsip.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry("bytes", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| file | java.io.File | the metadata of file or folder to be compressed |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final TarEntry createEntry(String name, String path)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
             archive.createEntry(first.bin, "data.bin");
             archive.save(outputTarFile);
     }
 
```

Nama entri hanya ditetapkan dalam parameter `name`. Nama file yang diberikan dalam parameter `path` tidak memengaruhi nama entri.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String | nama entri |
| path | java.lang.String | jalur ke file yang akan dikompresi |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final TarEntry createEntry(String name, String path, boolean openImmediately)
```


Membuat satu entri dalam arsip.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, "data.bin");
archive.save(outputTarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | path to file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### deleteEntry(TarEntry entry) {#deleteEntry-com.aspose.zip.TarEntry-}
```
public final TarArchive deleteEntry(TarEntry entry)
```


Removes the first occurrence of a specific entry from the entry list.

Here is how you can remove all entries except the last one:

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         while (archive.getEntries().size() > 1)
             archive.deleteEntry(archive.getEntries().get_Item(0));
         archive.save(outputTarFile);
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| entry | [TarEntry](../../com.aspose.zip/tarentry) | entri yang akan dihapus dari daftar entri |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final TarArchive deleteEntry(int entryIndex)
```


Menghapus entri dari daftar entri berdasarkan indeks.

```

``````

try (TarArchive archive = new TarArchive("two_files.tar")) {
archive.deleteEntry(0);
archive.save("single_file.tar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | int | the zero-based index of the entry to remove |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

Jika direktori tidak ada, maka akan dibuat.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationDirectory | java.lang.String | jalur ke direktori tempat menempatkan file yang diekstrak |

### fromGZip(InputStream source) {#fromGZip-java.io.InputStream-}
```
public static TarArchive fromGZip(InputStream source)
```


Mengekstrak arsip gzip yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak.

Penting: arsip gzip diekstrak sepenuhnya dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

Aliran ekstraksi GZip tidak dapat di-seek karena sifat algoritma kompresi. Arsip Tar menyediakan fasilitas untuk mengekstrak rekaman apa pun, sehingga harus beroperasi pada aliran yang dapat di-seek di balik layar.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | java.io.InputStream | sumber arsip. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromGZip(String path) {#fromGZip-java.lang.String-}
```
public static TarArchive fromGZip(String path)
```


Mengekstrak arsip gzip yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak.

Penting: arsip gzip diekstrak sepenuhnya dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

Aliran ekstraksi GZip tidak dapat di-seek karena sifat algoritma kompresi. Arsip Tar menyediakan fasilitas untuk mengekstrak rekaman apa pun, sehingga harus beroperasi pada aliran yang dapat di-seek di balik layar.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur ke file arsip. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(InputStream source) {#fromLZ4-java.io.InputStream-}
```
public static TarArchive fromLZ4(InputStream source)
```


Mengekstrak arsip LZ4 yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak.

Penting: arsip LZ4 diekstrak sepenuhnya dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | source | java.io.InputStream | Sumber arsip. |

Aliran ekstraksi LZ4 tidak dapat dicari karena sifat algoritma kompresi. Arsip Tar menyediakan fasilitas untuk mengekstrak rekaman apa saja, sehingga harus beroperasi pada aliran yang dapat dicari di balik layar. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(String path) {#fromLZ4-java.lang.String-}
```
public static TarArchive fromLZ4(String path)
```


Mengekstrak arsip LZ4 yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak.

Penting: arsip LZ4 diekstrak sepenuhnya dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | path | java.lang.String | Jalur ke file arsip. |

Aliran ekstraksi LZ4 tidak dapat dicari karena sifat algoritma kompresi. Arsip Tar menyediakan fasilitas untuk mengekstrak rekaman apa saja, sehingga harus beroperasi pada aliran yang dapat dicari di balik layar. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(InputStream source) {#fromLZMA-java.io.InputStream-}
```
public static TarArchive fromLZMA(InputStream source)
```


Mengekstrak arsip LZMA yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak.

Penting: arsip LZMA diekstrak sepenuhnya dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

Aliran ekstraksi LZMA tidak dapat dicari karena sifat algoritma kompresi. Arsip Tar menyediakan fasilitas untuk mengekstrak rekaman apa saja, sehingga harus beroperasi pada aliran yang dapat dicari di balik layar.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | java.io.InputStream | sumber arsip |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(String path) {#fromLZMA-java.lang.String-}
```
public static TarArchive fromLZMA(String path)
```


Mengekstrak arsip LZMA yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak.

Penting: arsip LZMA diekstrak sepenuhnya dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

Aliran ekstraksi LZMA tidak dapat dicari karena sifat algoritma kompresi. Arsip Tar menyediakan fasilitas untuk mengekstrak rekaman apa saja, sehingga harus beroperasi pada aliran yang dapat dicari di balik layar.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur ke file arsip |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(InputStream source) {#fromLZip-java.io.InputStream-}
```
public static TarArchive fromLZip(InputStream source)
```


Mengekstrak arsip lzip yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak.

Penting: arsip lzip diekstrak sepenuhnya dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

Aliran ekstraksi Lzip tidak dapat dicari karena sifat algoritma kompresi. Arsip Tar menyediakan fasilitas untuk mengekstrak rekaman apa saja, sehingga harus beroperasi pada aliran yang dapat dicari di balik layar

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | java.io.InputStream | sumber arsip. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(String path) {#fromLZip-java.lang.String-}
```
public static TarArchive fromLZip(String path)
```


Mengekstrak arsip lzip yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak.

Penting: arsip lzip diekstrak sepenuhnya dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

Aliran ekstraksi Lzip tidak dapat dicari karena sifat algoritma kompresi. Arsip Tar menyediakan fasilitas untuk mengekstrak rekaman apa saja, sehingga harus beroperasi pada aliran yang dapat dicari di balik layar

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur ke file arsip. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(InputStream source) {#fromXz-java.io.InputStream-}
```
public static TarArchive fromXz(InputStream source)
```


Mengekstrak arsip format xz yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak.

Penting: arsip xz diekstrak sepenuhnya dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

Arsip Tar menyediakan fasilitas untuk mengekstrak rekaman apa saja, sehingga harus beroperasi pada aliran yang dapat dicari di balik layar.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | java.io.InputStream | sumber arsip |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(String path) {#fromXz-java.lang.String-}
```
public static TarArchive fromXz(String path)
```


Mengekstrak arsip format xz yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak.

Penting: arsip xz diekstrak sepenuhnya dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

Arsip Tar menyediakan fasilitas untuk mengekstrak rekaman apa saja, sehingga harus beroperasi pada aliran yang dapat dicari di balik layar.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur ke file arsip |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(InputStream source) {#fromZ-java.io.InputStream-}
```
public static TarArchive fromZ(InputStream source)
```


Mengekstrak arsip format Z yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak.

Penting: arsip Z diekstrak sepenuhnya dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | java.io.InputStream | sumber arsip |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(String path) {#fromZ-java.lang.String-}
```
public static TarArchive fromZ(String path)
```


Mengekstrak arsip format Z yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak.

Penting: arsip Z diekstrak sepenuhnya dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur ke file arsip |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(InputStream source) {#fromZstandard-java.io.InputStream-}
```
public static TarArchive fromZstandard(InputStream source)
```


Mengekstrak arsip Zstandard yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak.

Penting: arsip Zstandard diekstrak sepenuhnya dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | java.io.InputStream | sumber arsip |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(String path) {#fromZstandard-java.lang.String-}
```
public static TarArchive fromZstandard(String path)
```


Mengekstrak arsip Zstandard yang diberikan dan menyusun [TarArchive](../../com.aspose.zip/tararchive) dari data yang diekstrak.

Penting: arsip Zstandard diekstrak sepenuhnya dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur ke file arsip |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### getEntries() {#getEntries--}
```
public final List<TarEntry> getEntries()
```


Mendapatkan entri tipe [TarEntry](../../com.aspose.zip/tarentry) yang membentuk arsip.

**Returns:**
java.util.List&lt;com.aspose.zip.TarEntry&gt; - entri dari tipe [TarEntry](../../com.aspose.zip/tarentry) yang membentuk arsip
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Mendapatkan entri tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip tar.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entri dari tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip tar
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Mendapatkan format arsip.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Menyimpan arsip ke aliran yang disediakan.

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### save(OutputStream output, TarFormat format) {#save-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void save(OutputStream output, TarFormat format)
```


Saves archive to the stream provided.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry1", "data.bin");
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | output | java.io.OutputStream | stream tujuan. |

`output` harus dapat ditulis |
| format | [TarFormat](../../com.aspose.zip/tarformat) | menentukan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Menyimpan arsip ke file tujuan yang disediakan.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save("myarchive.tar");
}
 
```

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### save(String destinationFileName, TarFormat format) {#save-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void save(String destinationFileName, TarFormat format)
```


Saves archive to the destination file provided.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("myarchive.tar");
     }
 
```

Dimungkinkan untuk menyimpan arsip ke jalur yang sama dengan tempat ia dimuat. Namun, ini tidak disarankan karena pendekatan ini menggunakan penyalinan ke file sementara

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationFileName | java.lang.String | jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | menentukan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan |

### saveGzipped(OutputStream output) {#saveGzipped-java.io.OutputStream-}
```
public final void saveGzipped(OutputStream output)
```


Menyimpan arsip ke aliran dengan kompresi gzip.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped(result);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveGzipped(OutputStream output, TarFormat format) {#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with gzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveGzipped(result);
             }
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | output | java.io.OutputStream | stream tujuan. |

`output` harus dapat ditulis |
| format | [TarFormat](../../com.aspose.zip/tarformat) | menentukan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan |

### saveGzipped(String path) {#saveGzipped-java.lang.String-}
```
public final void saveGzipped(String path)
```


Menyimpan arsip ke file berdasarkan jalur dengan kompresi gzip.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped("result.tar.gz");
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveGzipped(String path, TarFormat format) {#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(String path, TarFormat format)
```


Saves archive to the file by path with gzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveGzipped("result.tar.gz");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa |
| format | [TarFormat](../../com.aspose.zip/tarformat) | menentukan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan |

### saveLZ4Compressed(OutputStream output) {#saveLZ4Compressed-java.io.OutputStream-}
```
public final void saveLZ4Compressed(OutputStream output)
```


Menyimpan arsip ke aliran dengan kompresi LZ4.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | Destination stream. |

### saveLZ4Compressed(OutputStream output, TarFormat format) {#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZ4 compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZ4Compressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| output | java.io.OutputStream | Aliran tujuan. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Menentukan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan. |

### saveLZ4Compressed(String path) {#saveLZ4Compressed-java.lang.String-}
```
public final void saveLZ4Compressed(String path)
```


Menyimpan arsip ke file dengan jalur menggunakan kompresi LZ4.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed("result.tar.lz4");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### saveLZ4Compressed(String path, TarFormat format) {#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(String path, TarFormat format)
```


Saves archive to the file by path with LZ4 compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZ4Compressed("result.tar.lz4");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, maka akan ditimpa. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Menentukan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan. |

### saveLZMACompressed(OutputStream output) {#saveLZMACompressed-java.io.OutputStream-}
```
public final void saveLZMACompressed(OutputStream output)
```


Menyimpan arsip ke aliran dengan kompresi LZMA.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed(result);
}
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveLZMACompressed(OutputStream output, TarFormat format) {#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZMA compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZMACompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```

Penting: arsip tar disusun lalu dikompresi dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | output | java.io.OutputStream | stream tujuan. |

`output` harus dapat ditulis |
| format | [TarFormat](../../com.aspose.zip/tarformat) | menentukan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan |

### saveLZMACompressed(String path) {#saveLZMACompressed-java.lang.String-}
```
public final void saveLZMACompressed(String path)
```


Menyimpan arsip ke file dengan jalur menggunakan kompresi lzma.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed("result.tar.lzma");
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLZMACompressed(String path, TarFormat format) {#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(String path, TarFormat format)
```


Saves archive to the file by path with lzma compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZMACompressed("result.tar.lzma");
         }
     } catch (IOException ex) {
     }
 
```

Penting: arsip tar disusun lalu dikompresi dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa |
| format | [TarFormat](../../com.aspose.zip/tarformat) | menentukan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan |

### saveLzipped(OutputStream output) {#saveLzipped-java.io.OutputStream-}
```
public final void saveLzipped(OutputStream output)
```


Menyimpan arsip ke aliran dengan kompresi lzip.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
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

### saveLzipped(OutputStream output, TarFormat format) {#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with lzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLzipped(result, TarFormat.Gnu);
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
| format | [TarFormat](../../com.aspose.zip/tarformat) | menentukan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan |

### saveLzipped(String path) {#saveLzipped-java.lang.String-}
```
public final void saveLzipped(String path)
```


Menyimpan arsip ke file berdasarkan jalur dengan kompresi lzip.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped("result.tar.lz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLzipped(String path, TarFormat format) {#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(String path, TarFormat format)
```


Saves archive to the file by path with lzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLzipped("result.tar.lz", TarFormat.Gnu);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa |
| format | [TarFormat](../../com.aspose.zip/tarformat) | menentukan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan |

### saveXzCompressed(OutputStream output) {#saveXzCompressed-java.io.OutputStream-}
```
public final void saveXzCompressed(OutputStream output)
```


Menyimpan arsip ke aliran dengan kompresi xz.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
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

### saveXzCompressed(OutputStream output, TarFormat format) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
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
| format | [TarFormat](../../com.aspose.zip/tarformat) | menentukan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan |

### saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)
```


Menyimpan arsip ke aliran dengan kompresi xz.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
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
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines the tar header format. Null value will be treated as USTar when possible |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | set of setting particular xz archive: dictionary size, block size, check type |

### saveXzCompressed(String path) {#saveXzCompressed-java.lang.String-}
```
public final void saveXzCompressed(String path)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa |

### saveXzCompressed(String path, TarFormat format) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(String path, TarFormat format)
```


Menyimpan arsip ke file berdasarkan jalur dengan kompresi xz.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed("result.tar.xz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines tar header format. Null value will be treated as USTar when possible |

### saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa |
| format | [TarFormat](../../com.aspose.zip/tarformat) | menentukan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | sekumpulan pengaturan khusus arsip xz: ukuran kamus, ukuran blok, tipe pemeriksaan |

### saveZCompressed(OutputStream output) {#saveZCompressed-java.io.OutputStream-}
```
public final void saveZCompressed(OutputStream output)
```


Menyimpan arsip ke aliran dengan kompresi Z.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
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
| output | java.io.OutputStream | the destination stream |

### saveZCompressed(OutputStream output, TarFormat format) {#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with Z compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
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
| output | java.io.OutputStream | aliran tujuan |
| format | [TarFormat](../../com.aspose.zip/tarformat) | menentukan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan |

### saveZCompressed(String path) {#saveZCompressed-java.lang.String-}
```
public final void saveZCompressed(String path)
```


Menyimpan arsip ke file berdasarkan jalur dengan kompresi Z.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed("result.tar.Z");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZCompressed(String path, TarFormat format) {#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(String path, TarFormat format)
```


Saves archive to the file by path with Z compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZCompressed("result.tar.Z");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa |
| format | [TarFormat](../../com.aspose.zip/tarformat) | menentukan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan |

### saveZstandard(OutputStream output) {#saveZstandard-java.io.OutputStream-}
```
public final void saveZstandard(OutputStream output)
```


Menyimpan arsip ke aliran dengan kompresi Zstandard.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
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

### saveZstandard(OutputStream output, TarFormat format) {#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(OutputStream output, TarFormat format)
```


Saves archive to the stream with Zstandard compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
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
| format | [TarFormat](../../com.aspose.zip/tarformat) | menentukan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan |

### saveZstandard(String path) {#saveZstandard-java.lang.String-}
```
public final void saveZstandard(String path)
```


Menyimpan arsip ke file berdasarkan jalur dengan kompresi Zstandard.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard("result.tar.zst");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZstandard(String path, TarFormat format) {#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(String path, TarFormat format)
```


Saves archive to the file by path with Zstandard compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZstandard("result.tar.zst");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa |
| format | [TarFormat](../../com.aspose.zip/tarformat) | menentukan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan |

