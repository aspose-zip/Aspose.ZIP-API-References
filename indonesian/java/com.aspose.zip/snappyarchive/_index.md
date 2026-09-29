---
title: "SnappyArchive"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Kelas ini mewakili file arsip snappy."
type: docs
weight: 121
url: /id/java/com.aspose.zip/snappyarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class SnappyArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Kelas ini mewakili file arsip snappy. Gunakan untuk membuat atau mengekstrak arsip snappy.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [SnappyArchive()](#SnappyArchive--) | Menginisialisasi instance baru dari kelas [SnappyArchive](../../com.aspose.zip/snappyarchive) yang disiapkan untuk kompresi. |
| [SnappyArchive(InputStream source)](#SnappyArchive-java.io.InputStream-) | Menginisialisasi instance baru dari kelas [SnappyArchive](../../com.aspose.zip/snappyarchive) yang disiapkan untuk dekompresi. |
| [SnappyArchive(String path)](#SnappyArchive-java.lang.String-) | Menginisialisasi instance baru dari kelas [SnappyArchive](../../com.aspose.zip/snappyarchive) yang disiapkan untuk dekompresi. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Mengekstrak arsip snappy ke sebuah file. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Mengekstrak arsip snappy ke sebuah aliran. |
| [extract(String path)](#extract-java.lang.String-) | Mengekstrak arsip snappy ke file berdasarkan jalur. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Mengekstrak konten arsip ke direktori yang diberikan. |
| [getFileEntries()](#getFileEntries--) | Mendapatkan entri tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip snappy. |
| [getFormat()](#getFormat--) | Mendapatkan format arsip. |
| [getLength()](#getLength--) | Mendapatkan panjang. |
| [getName()](#getName--) | Nama file asli. |
| [save(File destination)](#save-java.io.File-) | Menyimpan arsip snappy ke file tujuan yang diberikan. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Menyimpan arsip snappy ke aliran yang diberikan |
| [save(String destinationFileName)](#save-java.lang.String-) | Menyimpan arsip snappy ke file tujuan yang diberikan. |
| [setSource(File file)](#setSource-java.io.File-) | Mengatur konten yang akan dikompresi dalam arsip. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Mengatur konten yang akan dikompresi dalam arsip. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Mengatur konten yang akan dikompresi dalam arsip. |
### SnappyArchive() {#SnappyArchive--}
```
public SnappyArchive()
```


Menginisialisasi instance baru dari kelas [SnappyArchive](../../com.aspose.zip/snappyarchive) yang disiapkan untuk kompresi.

Contoh berikut menunjukkan cara mengompresi sebuah file.

```

``````

try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource("data.bin");
archive.save("archive.snappy");
}
 
```



### SnappyArchive(InputStream source) {#SnappyArchive-java.io.InputStream-}
```
public SnappyArchive(InputStream source)
```


Initializes a new instance of the [SnappyArchive](../../com.aspose.zip/snappyarchive) class prepared for decompressing.

This constructor does not decompress. See [extract(java.io.OutputStream)](../../com.aspose.zip/snappyarchive\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | The source of the archive. |

### SnappyArchive(String path) {#SnappyArchive-java.lang.String-}
```
public SnappyArchive(String path)
```


Initializes a new instance of the [SnappyArchive](../../com.aspose.zip/snappyarchive) class prepared for decompressing.

```

``````

      try (FileInputStream sourceSnappyFile = new FileInputStream("sourceFileName")) {
          try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
              try (SnappyArchive archive = new SnappyArchive(sourceSnappyFile)) {
                  archive.extract(extractedFile);
              }
          }
      } catch (IOException ex) {
      }
 
```

Konstruktor ini tidak melakukan dekompresi. Lihat metode [extract(java.io.OutputStream)](../../com.aspose.zip/snappyarchive\#extract-java.io.OutputStream-) untuk dekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur ke sumber arsip |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Mengekstrak arsip snappy ke sebuah file.

```

``````

try (FileInputStream snappyFile = new FileInputStream("sourceFileName")) {
try (SnappyArchive archive = new SnappyArchive(snappyFile)) {
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


Extracts snappy archive to a stream.

```

``````

     try (FileInputStream sourceSnappyFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (SnappyArchive archive = new SnappyArchive(sourceSnappyFile)) {
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


Mengekstrak arsip snappy ke file berdasarkan jalur.

```

``````

try (FileInputStream snappyFile = new FileInputStream("sourceFileName")) {
try (SnappyArchive archive = new SnappyArchive(snappyFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file which will store decompressed data |

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

If the directory does not exist, it will be created |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the snappy archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the snappy archive
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


Gets length.

**Returns:**
java.lang.Long - length.
### getName() {#getName--}
```
public final String getName()
```


The name of original file.

**Returns:**
java.lang.String - the name of the original file
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves snappy archive to the destination file provided.

```

``````

     try (SnappyArchive archive = new SnappyArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.snappy"));
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tujuan | java.io.File | file, yang akan dibuka sebagai stream tujuan |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Menyimpan arsip snappy ke aliran yang diberikan

```

``````

try (FileOutputStream snappyFile = new FileOutputStream("archive.snappy")) {
try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource("data.bin");
archive.save(snappyFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves snappy archive to the destination file provided.

```

``````

     try (SnappyArchive archive = new SnappyArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.snappy");
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationFileName | java.lang.String | jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Mengatur konten yang akan dikompresi dalam arsip.

```

``````

try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("archive.snappy");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file which will be opened as an input stream |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (SnappyArchive archive = new SnappyArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.snappy");
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | java.io.InputStream | stream input untuk arsip |

### setSource(String sourcePath) {#setSource-java.lang.String-}
```
public final void setSource(String sourcePath)
```


Mengatur konten yang akan dikompresi dalam arsip.

```

``````

try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource("data.bin");
archive.save("archive.snappy");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourcePath | java.lang.String | the path to the file which will be opened as an input stream |

