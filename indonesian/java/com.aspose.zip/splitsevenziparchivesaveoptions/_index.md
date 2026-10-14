---
title: "SplitSevenZipArchiveSaveOptions"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Opsi untuk menyimpan arsip 7-zip multi-volume."
type: docs
weight: 123
url: /id/java/com.aspose.zip/splitsevenziparchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitSevenZipArchiveSaveOptions
```

Opsi untuk menyimpan arsip 7-zip multi-volume.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)](#SplitSevenZipArchiveSaveOptions-java.lang.String-long-) | Membuat instance pengaturan untuk menyimpan arsip 7z multi-volume. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getFileName()](#getFileName--) | Mendapatkan nama segmen tanpa ekstensi. |
| [getSegmentSize()](#getSegmentSize--) | Mendapatkan ukuran segmen. |
### SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize) {#SplitSevenZipArchiveSaveOptions-java.lang.String-long-}
```
public SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)
```


Membuat instance pengaturan untuk menyimpan arsip 7z multi-volume.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | fileName | java.lang.String | nama untuk volume. Bisa dengan atau tanpa ekstensi .7z. |

Nama file akan menjadi sebagai berikut: `fileName`.7z.001, `fileName`.7z.002, ..., `fileName`.7z.(n). |
|  | segmentSize | long | ukuran volume. |

Beberapa volume mungkin lebih kecil dari `segmentSize`. Dalam kebanyakan kasus, segmen terakhir akan lebih kecil tetapi jarang segmen reguler mungkin terlalu besar. |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Mendapatkan nama segmen tanpa ekstensi.

**Returns:**
java.lang.String - nama segmen tanpa ekstensi
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Mendapatkan ukuran segmen.

**Returns:**
long - ukuran segmen.
