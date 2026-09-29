---
title: "XzArchive"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Kelas ini mewakili berkas arsip xz."
type: docs
weight: 146
url: /id/java/com.aspose.zip/xzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class XzArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

Kelas ini merepresentasikan file arsip xz. Gunakan untuk menyusun dan mengekstrak arsip xz.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [XzArchive()](#XzArchive--) | Menginisialisasi sebuah instance baru dari kelas [XzArchive](../../com.aspose.zip/xzarchive) dan menyusun arsip dalam format xz. |
| [XzArchive(XzArchiveSettings settings)](#XzArchive-com.aspose.zip.XzArchiveSettings-) | Menginisialisasi sebuah instance baru dari kelas [XzArchive](../../com.aspose.zip/xzarchive) dan menyusun arsip dalam format xz. |
| [XzArchive(InputStream source)](#XzArchive-java.io.InputStream-) | Menginisialisasi sebuah instance baru dari kelas [XzArchive](../../com.aspose.zip/xzarchive) yang dipersiapkan untuk dekompresi. |
| [XzArchive(InputStream source, XzLoadOptions options)](#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-) | Menginisialisasi sebuah instance baru dari kelas [XzArchive](../../com.aspose.zip/xzarchive) yang dipersiapkan untuk dekompresi. |
| [XzArchive(String path)](#XzArchive-java.lang.String-) | Menginisialisasi sebuah instance baru dari kelas [XzArchive](../../com.aspose.zip/xzarchive) yang dipersiapkan untuk dekompresi. |
| [XzArchive(String path, XzLoadOptions options)](#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-) | Menginisialisasi sebuah instance baru dari kelas [XzArchive](../../com.aspose.zip/xzarchive) yang dipersiapkan untuk dekompresi. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Mengekstrak arsip xz ke sebuah file. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Mengekstrak arsip xz ke sebuah aliran. |
| [extract(String path)](#extract-java.lang.String-) | Mengekstrak arsip xz ke file berdasarkan jalur. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Mengekstrak konten arsip ke direktori yang diberikan. |
| [getFileEntries()](#getFileEntries--) | Mendapatkan entri tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip xz. |
| [getFormat()](#getFormat--) | Mendapatkan format arsip. |
| [getLength()](#getLength--) | Mendapatkan panjang entri dalam byte. |
| [getName()](#getName--) | Mendapatkan nama entri di dalam arsip. |
| [getUncompressedSize()](#getUncompressedSize--) | Mendapatkan ukuran data file yang tidak terkompresi dalam byte. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Menyimpan arsip xz ke aliran yang disediakan. |
| [save(String destinationFileName)](#save-java.lang.String-) | Menyimpan arsip xz ke file tujuan yang disediakan. |
| [setSource(File file)](#setSource-java.io.File-) | Mengatur konten yang akan dikompresi dalam arsip. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Mengatur konten yang akan dikompresi dalam arsip. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Mengatur konten yang akan dikompresi dalam arsip. |
### XzArchive() {#XzArchive--}
```
public XzArchive()
```


Menginisialisasi sebuah instance baru dari kelas [XzArchive](../../com.aspose.zip/xzarchive) dan menyusun arsip dalam format xz.

### XzArchive(XzArchiveSettings settings) {#XzArchive-com.aspose.zip.XzArchiveSettings-}
```
public XzArchive(XzArchiveSettings settings)
```


Menginisialisasi sebuah instance baru dari kelas [XzArchive](../../com.aspose.zip/xzarchive) dan menyusun arsip dalam format xz.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | sekumpulan pengaturan khusus arsip xz: ukuran kamus, ukuran blok, tipe pemeriksaan |

### XzArchive(InputStream source) {#XzArchive-java.io.InputStream-}
```
public XzArchive(InputStream source)
```


Menginisialisasi sebuah instance baru dari kelas [XzArchive](../../com.aspose.zip/xzarchive) yang dipersiapkan untuk dekompresi.

Konstruktor ini tidak melakukan dekompresi. Lihat metode [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) untuk dekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | java.io.InputStream | sumber arsip |

### XzArchive(InputStream source, XzLoadOptions options) {#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(InputStream source, XzLoadOptions options)
```


Menginisialisasi sebuah instance baru dari kelas [XzArchive](../../com.aspose.zip/xzarchive) yang dipersiapkan untuk dekompresi.

Konstruktor ini tidak melakukan dekompresi. Lihat metode [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) untuk dekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | java.io.InputStream | sumber arsip |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) | Opsi untuk memuat arsip dengan. |

### XzArchive(String path) {#XzArchive-java.lang.String-}
```
public XzArchive(String path)
```


Menginisialisasi sebuah instance baru dari kelas [XzArchive](../../com.aspose.zip/xzarchive) yang dipersiapkan untuk dekompresi.

Konstruktor ini tidak melakukan dekompresi. Lihat metode [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) untuk dekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur ke sumber arsip |

### XzArchive(String path, XzLoadOptions options) {#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(String path, XzLoadOptions options)
```


Menginisialisasi sebuah instance baru dari kelas [XzArchive](../../com.aspose.zip/xzarchive) yang dipersiapkan untuk dekompresi.

Konstruktor ini tidak melakukan dekompresi. Lihat metode [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) untuk dekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur ke sumber arsip |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) |  |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Mengekstrak arsip xz ke sebuah file.

```

``````

coba (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
coba (XzArchive archive = new XzArchive(xzFile)) {
archive.extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts xz archive to a stream.

```

``````

     try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (XzArchive archive = new XzArchive(xzFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tujuan | java.io.OutputStream | aliran untuk menyimpan data yang telah didekompresi |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Mengekstrak arsip xz ke file berdasarkan jalur.

```

``````

coba (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
coba (XzArchive archive = new XzArchive(xzFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | path to file which will store decompressed data |

**Returns:**
java.io.File - java.io.File instance containing extracted data
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within archive.

**Returns:**
java.lang.String - the name of the entry within archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the file data in bytes.

**Returns:**
long - the uncompressed size of the file data in bytes
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves xz archive to the stream provided.

```

``````

     try (FileOutputStream xzFile = new FileOutputStream("archive.xz")) {
         try (XzArchive archive = new XzArchive()) {
             archive.setSource("data.bin");
             archive.save(xzFile);
         }
     } catch (IOException ex) {
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


Menyimpan arsip xz ke file tujuan yang disediakan.

```

``````

coba (XzArchive archive = new XzArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("result.xz");
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

     try (XzArchive archive = new XzArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.xz");
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

coba (XzArchive archive = new XzArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.xz");
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

     try (XzArchive archive = new XzArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourcePath | java.lang.String | jalur ke file yang akan dibuka sebagai aliran masukan |

