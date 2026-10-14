---
title: "LzmaArchive"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Kelas ini mewakili file arsip LZMA."
type: docs
weight: 86
url: /id/java/com.aspose.zip/lzmaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzmaArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Kelas ini mewakili file arsip LZMA. Gunakan untuk membuat atau mengekstrak arsip LZMA.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [LzmaArchive()](#LzmaArchive--) | Menginisialisasi sebuah instance baru dari kelas [LzmaArchive](../../com.aspose.zip/lzmaarchive) dan menyusun arsip dalam format lzma. |
| [LzmaArchive(LzmaArchiveSettings settings)](#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-) | Menginisialisasi sebuah instance baru dari kelas [LzmaArchive](../../com.aspose.zip/lzmaarchive) dan menyusun arsip dalam format lzma. |
| [LzmaArchive(InputStream source)](#LzmaArchive-java.io.InputStream-) | Menginisialisasi sebuah instance baru dari kelas [LzmaArchive](../../com.aspose.zip/lzmaarchive) yang disiapkan untuk dekompresi. |
| [LzmaArchive(String path)](#LzmaArchive-java.lang.String-) | Menginisialisasi sebuah instance baru dari kelas [LzmaArchive](../../com.aspose.zip/lzmaarchive) yang disiapkan untuk dekompresi. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Mengekstrak arsip lzma ke sebuah file. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Mengekstrak arsip lzma ke sebuah stream. |
| [extract(String path)](#extract-java.lang.String-) | Mengekstrak arsip lzma ke file berdasarkan path. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Mengekstrak konten arsip ke direktori yang diberikan. |
| [getFileEntries()](#getFileEntries--) | Mendapatkan entri tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip lzma. |
| [getFormat()](#getFormat--) | Mendapatkan format arsip. |
| [getLength()](#getLength--) | Mendapatkan panjang. |
| [getName()](#getName--) | Nama file asli. |
| [save(File destination)](#save-java.io.File-) | Menyimpan arsip lzma ke file tujuan yang diberikan. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Menyimpan arsip lzma ke aliran yang disediakan. |
| [save(String destinationFileName)](#save-java.lang.String-) | Menyimpan arsip lzma ke file tujuan yang diberikan. |
| [setSource(File file)](#setSource-java.io.File-) | Mengatur konten yang akan dikompresi dalam arsip. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Mengatur konten yang akan dikompresi dalam arsip. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Mengatur konten yang akan dikompresi dalam arsip. |
### LzmaArchive() {#LzmaArchive--}
```
public LzmaArchive()
```


Menginisialisasi sebuah instance baru dari kelas [LzmaArchive](../../com.aspose.zip/lzmaarchive) dan menyusun arsip dalam format lzma.

### LzmaArchive(LzmaArchiveSettings settings) {#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-}
```
public LzmaArchive(LzmaArchiveSettings settings)
```


Menginisialisasi sebuah instance baru dari kelas [LzmaArchive](../../com.aspose.zip/lzmaarchive) dan menyusun arsip dalam format lzma.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| settings | [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) | kumpulan pengaturan arsip lzma tertentu |

### LzmaArchive(InputStream source) {#LzmaArchive-java.io.InputStream-}
```
public LzmaArchive(InputStream source)
```


Menginisialisasi sebuah instance baru dari kelas [LzmaArchive](../../com.aspose.zip/lzmaarchive) yang disiapkan untuk dekompresi.

Konstruktor ini tidak melakukan dekompresi. Lihat metode [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) untuk dekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | java.io.InputStream | sumber arsip |

### LzmaArchive(String path) {#LzmaArchive-java.lang.String-}
```
public LzmaArchive(String path)
```


Menginisialisasi sebuah instance baru dari kelas [LzmaArchive](../../com.aspose.zip/lzmaarchive) yang disiapkan untuk dekompresi.

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extracts lzma archive to a file.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract(new File("extracted.bin"));
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| file | java.io.File | file untuk menyimpan data yang didekompresi |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Mengekstrak arsip lzma ke sebuah stream.

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | the stream for storing decompressed data |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts lzma archive to a file by path.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract("extracted.bin");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | path ke file yang akan menyimpan data terdekompresi |

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
|  | destinationDirectory | java.lang.String | jalur ke direktori untuk menempatkan file yang diekstrak. |

Jika direktori tidak ada, maka akan dibuat |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Mendapatkan entri tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip lzma.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entri dari tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip lzma.
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


Mendapatkan panjang.

**Returns:**
java.lang.Long - panjang
### getName() {#getName--}
```
public final String getName()
```


Nama file asli.

**Returns:**
java.lang.String - nama file asli
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Menyimpan arsip lzma ke file tujuan yang diberikan.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(new File(\"archive.lzma\"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | the file, which will be opened as destination stream |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves lzma archive to the stream provided.

```

``````

     try (FileOutputStream lzmaFile = new FileOutputStream("archive.lzma")) {
         try (LzmaArchive archive = new LzmaArchive()) {
             archive.setSource("data.bin");
             archive.save(lzmaFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| output | java.io.OutputStream | stream tujuan |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Menyimpan arsip lzma ke file tujuan yang diberikan.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(\"result.lzma\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| file | java.io.File | file, yang akan dibuka sebagai aliran masukan |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Mengatur konten yang akan dikompresi dalam arsip.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save(\"archive.lzma\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String sourcePath) {#setSource-java.lang.String-}
```
public final void setSource(String sourcePath)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourcePath | java.lang.String | jalur ke file, yang akan dibuka sebagai aliran masukan |

