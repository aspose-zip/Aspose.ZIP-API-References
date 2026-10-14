---
title: "SplitArchiveSaveOptions"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Opsi untuk menyimpan arsip ZIP multi-volume."
type: docs
weight: 122
url: /id/java/com.aspose.zip/splitarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitArchiveSaveOptions
```

Opsi untuk menyimpan arsip ZIP multi-volume.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [SplitArchiveSaveOptions(String fileName, long segmentSize)](#SplitArchiveSaveOptions-java.lang.String-long-) | Membuat instance pengaturan untuk menyimpan arsip ZIP multi-volume. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Mendapatkan komentar opsional untuk file Zip. |
| [getCloseEntrySource()](#getCloseEntrySource--) | Mendapatkan nilai yang menunjukkan apakah sumber entri harus ditutup segera setelah entri dikompresi. |
| [getEncoding()](#getEncoding--) | Mendapatkan enkoding untuk mengonversi nama file dan string lainnya menjadi byte. |
| [getEventsBag()](#getEventsBag--) | Mendapatkan kontainer peristiwa yang dipicu saat menyimpan arsip. |
| [getFileName()](#getFileName--) | Mendapatkan nama segmen tanpa ekstensi. |
| [getSegmentSize()](#getSegmentSize--) | Mendapatkan ukuran segmen. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Mengatur komentar opsional untuk file Zip. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | Mengatur nilai yang menunjukkan apakah sumber entri harus ditutup segera setelah entri dikompresi. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Mengatur enkoding untuk mengonversi nama file dan string lainnya menjadi byte. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | Mengatur kontainer peristiwa yang dipicu saat menyimpan arsip. |
### SplitArchiveSaveOptions(String fileName, long segmentSize) {#SplitArchiveSaveOptions-java.lang.String-long-}
```
public SplitArchiveSaveOptions(String fileName, long segmentSize)
```


Membuat instance pengaturan untuk menyimpan arsip ZIP multi-volume.

Beberapa volume mungkin lebih kecil dari `segmentSize`. Dalam kebanyakan kasus, segmen terakhir akan lebih kecil tetapi jarang segmen reguler mungkin terlalu kecil.

Nama file akan menjadi sebagai berikut: `fileName`.z01, `fileName`.z02, ..., `fileName`.z(n-1), `fileName`.zip.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | java.lang.String | Nama untuk volume. Bisa dengan atau tanpa ekstensi .zip. |
| segmentSize | long | Ukuran volume. |

### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Mendapatkan komentar opsional untuk file Zip.

**Returns:**
java.lang.String - komentar opsional untuk file Zip.
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


Mendapatkan nilai yang menunjukkan apakah sumber entri harus ditutup segera setelah entri dikompresi.

**Returns:**
boolean - nilai yang menunjukkan apakah sumber entri harus ditutup segera setelah sebuah entri dikompresi.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Mendapatkan enkoding untuk mengonversi nama file dan string lainnya menjadi byte.

Jika tidak disetel, kode halaman 437 akan digunakan.

**Returns:**
java.nio.charset.Charset - pengkodean untuk mengonversi nama file dan string lainnya menjadi byte.
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


Mendapatkan kontainer peristiwa yang dipicu saat menyimpan arsip.

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getFileName() {#getFileName--}
```
public final String getFileName()
```


Mendapatkan nama segmen tanpa ekstensi.

**Returns:**
java.lang.String - nama segmen tanpa ekstensi.
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Mendapatkan ukuran segmen.

**Returns:**
long - ukuran segmen.
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


Mengatur komentar opsional untuk file Zip.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | komentar opsional untuk file Zip. |

### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


Mengatur nilai yang menunjukkan apakah sumber entri harus ditutup segera setelah entri dikompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah sumber entri harus ditutup segera setelah sebuah entri dikompresi. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Mengatur enkoding untuk mengonversi nama file dan string lainnya menjadi byte.

Jika tidak disetel, kode halaman 437 akan digunakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.nio.charset.Charset | encoding untuk mengonversi nama file dan string lain menjadi byte. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


Mengatur kontainer peristiwa yang dipicu saat menyimpan arsip.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | kontainer peristiwa yang dipicu saat menyimpan arsip. |

