---
title: "ZArchive"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Kelas ini mewakili file arsip Z compress."
type: docs
weight: 153
url: /id/java/com.aspose.zip/zarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ZArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

Kelas ini mewakili file arsip Z (compress). Gunakan untuk menyusun atau mengekstrak arsip Z.

Lihat [Z Compressed File Format ][Z Compressed File Format]


[Z Compressed File Format]: https://docs.fileformat.com/compression/z/
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ZArchive()](#ZArchive--) | Menginisialisasi instance baru dari kelas [ZArchive](../../com.aspose.zip/zarchive) yang disiapkan untuk kompresi. |
| [ZArchive(InputStream source)](#ZArchive-java.io.InputStream-) | Menginisialisasi instance baru dari kelas [ZArchive](../../com.aspose.zip/zarchive) yang disiapkan untuk dekompresi. |
| [ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)](#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-) | Menginisialisasi instance baru dari kelas [ZArchive](../../com.aspose.zip/zarchive) yang disiapkan untuk dekompresi. |
| [ZArchive(String path)](#ZArchive-java.lang.String-) | Menginisialisasi instance baru dari kelas [ZArchive](../../com.aspose.zip/zarchive) yang disiapkan untuk dekompresi. |
| [ZArchive(String path, ZArchiveLoadOptions loadOptions)](#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-) | Menginisialisasi instance baru dari kelas [ZArchive](../../com.aspose.zip/zarchive) yang disiapkan untuk dekompresi. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Mengekstrak arsip Z ke sebuah file. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Mengekstrak arsip Z ke aliran. |
| [extract(String path)](#extract-java.lang.String-) | Mengekstrak arsip Z ke file berdasarkan jalur. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Mengekstrak konten arsip ke direktori yang diberikan. |
| [getFileEntries()](#getFileEntries--) | Mendapatkan entri tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip Z. |
| [getFormat()](#getFormat--) | Mendapatkan format arsip. |
| [getLength()](#getLength--) | Mendapatkan panjang entri dalam byte. |
| [getName()](#getName--) | Mendapatkan nama entri di dalam arsip. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Menyimpan arsip Z ke aliran yang disediakan. |
| [save(OutputStream output, ZArchiveSaveOptions settings)](#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-) | Menyimpan arsip Z ke aliran yang disediakan. |
| [save(String destinationFileName)](#save-java.lang.String-) | Menyimpan arsip Z ke file tujuan yang diberikan. |
| [save(String destinationFileName, ZArchiveSaveOptions settings)](#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-) | Menyimpan arsip Z ke file tujuan yang diberikan. |
| [setSource(File file)](#setSource-java.io.File-) | Mengatur konten yang akan dikompresi dalam arsip. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Mengatur konten yang akan dikompresi dalam arsip. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Mengatur konten yang akan dikompresi dalam arsip. |
### ZArchive() {#ZArchive--}
```
public ZArchive()
```


Menginisialisasi instance baru dari kelas [ZArchive](../../com.aspose.zip/zarchive) yang disiapkan untuk kompresi.

### ZArchive(InputStream source) {#ZArchive-java.io.InputStream-}
```
public ZArchive(InputStream source)
```


Menginisialisasi instance baru dari kelas [ZArchive](../../com.aspose.zip/zarchive) yang disiapkan untuk dekompresi.

Konstruktor ini tidak melakukan dekompresi. Lihat metode [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) untuk dekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | java.io.InputStream | sumber arsip |

### ZArchive(InputStream source, ZArchiveLoadOptions loadOptions) {#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)
```


Menginisialisasi instance baru dari kelas [ZArchive](../../com.aspose.zip/zarchive) yang disiapkan untuk dekompresi.

Konstruktor ini tidak melakukan dekompresi. Lihat metode [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) untuk dekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | java.io.InputStream | sumber arsip |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | opsi untuk memuat arsip dengan |

### ZArchive(String path) {#ZArchive-java.lang.String-}
```
public ZArchive(String path)
```


Menginisialisasi instance baru dari kelas [ZArchive](../../com.aspose.zip/zarchive) yang disiapkan untuk dekompresi.

Konstruktor ini tidak melakukan dekompresi. Lihat metode [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) untuk dekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur ke sumber arsip |

### ZArchive(String path, ZArchiveLoadOptions loadOptions) {#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(String path, ZArchiveLoadOptions loadOptions)
```


Menginisialisasi instance baru dari kelas [ZArchive](../../com.aspose.zip/zarchive) yang disiapkan untuk dekompresi.

Konstruktor ini tidak melakukan dekompresi. Lihat metode [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) untuk dekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur ke sumber arsip |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | opsi untuk memuat arsip dengan |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Mengekstrak arsip Z ke sebuah file.

```

``````

try (FileInputStream zFile = new FileInputStream(\"sourceFileName\")) {
try (ZArchive archive = new ZArchive(zFile)) {
archive.extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts Z archive to a stream.

```

``````

     try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (ZArchive archive = new ZArchive(zFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tujuan | java.io.OutputStream | stream untuk menyimpan data yang didekompresi |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Mengekstrak arsip Z ke file berdasarkan jalur.

```

``````

try (FileInputStream zFile = new FileInputStream(\"sourceFileName\")) {
try (ZArchive archive = new ZArchive(zFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to file which will store decompressed data |

**Returns:**
java.io.File - the file info of the extracted file
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive
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
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves Z archive to the stream provided.

```

``````

     try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
         try (ZArchive archive = new ZArchive()) {
             archive.setSource("data.bin");
             archive.save(zFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| output | java.io.OutputStream | aliran tujuan |

### save(OutputStream output, ZArchiveSaveOptions settings) {#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(OutputStream output, ZArchiveSaveOptions settings)
```


Menyimpan arsip Z ke aliran yang disediakan.

```

``````

try (FileOutputStream zFile = new FileOutputStream(\"data.bin.Z\")) {
try (ZArchive archive = new ZArchive()) {
archive.setSource("data.bin");
archive.save(zFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves Z archive to the destination file provided.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationFileName | java.lang.String | jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa |

### save(String destinationFileName, ZArchiveSaveOptions settings) {#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(String destinationFileName, ZArchiveSaveOptions settings)
```


Menyimpan arsip Z ke file tujuan yang diberikan.

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(\"data.bin.Z\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| file | java.io.File | informasi file yang akan dibuka sebagai aliran masukan |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Mengatur konten yang akan dikompresi dalam arsip.

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save(\"archive.Z\");
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

     try (ZArchive archive = new ZArchive()) {
         archive.setSource("data.bin");
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourcePath | java.lang.String | jalur ke file yang akan dibuka sebagai aliran masukan |

