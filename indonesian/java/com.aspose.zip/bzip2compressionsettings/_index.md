---
title: "Bzip2CompressionSettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan untuk kompresi Bzip2 dalam arsip ZIP."
type: docs
weight: 41
url: /id/java/com.aspose.zip/bzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class Bzip2CompressionSettings extends CompressionSettings
```

Pengaturan untuk kompresi Bzip2 dalam arsip ZIP.

bzip2 mengompresi file menggunakan algoritma kompresi teks penyortiran blok Burrows-Wheeler, dan pengkodean Huffman.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Bzip2CompressionSettings(int blockSize)](#Bzip2CompressionSettings-int-) | Menginisialisasi sebuah instance baru dari kelas [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings). |
| [Bzip2CompressionSettings()](#Bzip2CompressionSettings--) | Menginisialisasi sebuah instance baru dari kelas [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) dengan ukuran blok default, yaitu 9 ratus kilobyte. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Ukuran blok dalam ratus kilobyte. |
### Bzip2CompressionSettings(int blockSize) {#Bzip2CompressionSettings-int-}
```
public Bzip2CompressionSettings(int blockSize)
```


Menginisialisasi sebuah instance baru dari kelas [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1)))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | Block size in hundreds of kilobytes. |

### Bzip2CompressionSettings() {#Bzip2CompressionSettings--}
```
public Bzip2CompressionSettings()
```


Initializes a new instance of the [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) class with default block size, equals to 9 hundred of kilobytes.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save(zipFile);
     }
 
```



### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Ukuran blok dalam ratus kilobyte.

**Returns:**
int - ukuran blok dalam ratus kilobyte
