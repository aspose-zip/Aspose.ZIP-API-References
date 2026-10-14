---
title: "XzArchiveSettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Kelas ini berisi sekumpulan pengaturan arsip xz tertentu."
type: docs
weight: 147
url: /id/java/com.aspose.zip/xzarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class XzArchiveSettings
```

Kelas ini berisi sekumpulan pengaturan arsip xz tertentu.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [XzArchiveSettings()](#XzArchiveSettings--) | Menginisialisasi sebuah instance baru dari kelas [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) menggunakan kompresi LZMA2 tunggal. |
| [XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)](#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-) | Menginisialisasi sebuah instance baru dari kelas [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) dengan parameter khusus. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Mendapatkan jumlah thread kompresi. |
| [getFastSpeed()](#getFastSpeed--) | Mendapatkan instance dari kelas [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) dengan ukuran kamus sebesar 1 megabyte pada filter LZMA2, ukuran blok sebesar 4 megabyte, dan checksum CRC32. |
| [getFastestSpeed()](#getFastestSpeed--) | Mendapatkan instance dari kelas [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) dengan ukuran kamus sebesar 65536 byte pada filter LZMA2, ukuran blok sebesar 1 megabyte, dan checksum CRC32. |
| [getHighCompression()](#getHighCompression--) | Mendapatkan instance dari kelas [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) dengan ukuran kamus sebesar 32 megabyte pada filter LZMA2, ukuran blok sebesar 128 megabyte, dan checksum CRC32. |
| [getMaximumCompression()](#getMaximumCompression--) | Mendapatkan instance dari kelas [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) dengan ukuran kamus sebesar 64 megabyte pada filter LZMA2, ukuran blok sebesar 256 megabyte, dan checksum CRC32. |
| [getNormal()](#getNormal--) | Mendapatkan instance dari kelas [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) dengan ukuran kamus sebesar 16 megabyte pada filter LZMA2, ukuran blok sebesar 64 megabyte, dan checksum CRC32. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Mengatur jumlah thread kompresi. |
### XzArchiveSettings() {#XzArchiveSettings--}
```
public XzArchiveSettings()
```


Menginisialisasi sebuah instance baru dari kelas [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) menggunakan kompresi LZMA2 tunggal.

Kamus default pada filter LZMA2 berukuran 16 megabyte, ukuran blok default 64 megabyte, tipe checksum default adalah CRC32.

### XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType) {#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-}
```
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```


Menginisialisasi sebuah instance baru dari kelas [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) dengan parameter khusus.

```

``````

try (FileOutputStream xzFile = new FileOutputStream("archive.xz")) {
XzLZMA2FilterSettings filter = new XzLZMA2FilterSettings(5242880);
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {filter}, 10485760, XzCheckType.Crc32);
try (XzArchive archive = new XzArchive(settings)) {
archive.setSource("data.bin");
archive.save(xzFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filters | [XzFilterSettings\[\]](../../com.aspose.zip/xzfiltersettings) | filters (compressors) to be sequentially applied to create [XzArchive](../../com.aspose.zip/xzarchive). It can be either single [XzLZMA2FilterSettings](../../com.aspose.zip/xzlzma2filtersettings) or pair of [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings) and [XzLZMA2FilterSettings](../../com.aspose.zip/xzlzma2filtersettings) |
| blockSize | long | size xz archive block |
| checkType | [XzCheckType](../../com.aspose.zip/xzchecktype) | type of checksum calculation for uncompressed data |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Gets compression thread count. If the value is greater than 1, multithreading compression will be used.

**Returns:**
int - compression thread count.
### getFastSpeed() {#getFastSpeed--}
```
public static XzArchiveSettings getFastSpeed()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 1 megabyte in LZMA2 filter, block size equals to 4 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the fast speed
### getFastestSpeed() {#getFastestSpeed--}
```
public static XzArchiveSettings getFastestSpeed()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 65536 bytes in LZMA2 filter, block size equals to 1 megabyte and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the fastest speed
### getHighCompression() {#getHighCompression--}
```
public static XzArchiveSettings getHighCompression()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 32 megabytes in LZMA2 filter, block size equals to 128 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the high compression
### getMaximumCompression() {#getMaximumCompression--}
```
public static XzArchiveSettings getMaximumCompression()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 64 megabytes in LZMA2 filter, block size equals to 256 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the maximum compression
### getNormal() {#getNormal--}
```
public static XzArchiveSettings getNormal()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 16 megabytes in LZMA2 filter, block size equals to 64 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with normal parameters
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Sets compression thread count. If the value is greater than 1, multithreading compression will be used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | compression thread count.

Do not set this number more than CPU cores |

