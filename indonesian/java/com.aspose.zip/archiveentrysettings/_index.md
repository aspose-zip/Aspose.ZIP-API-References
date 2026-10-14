---
title: "ArchiveEntrySettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan yang digunakan untuk mengompresi atau mendekompresi entri."
type: docs
weight: 30
url: /id/java/com.aspose.zip/archiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveEntrySettings
```

Pengaturan yang digunakan untuk mengompresi atau mendekompresi entri.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ArchiveEntrySettings()](#ArchiveEntrySettings--) | Menginisialisasi sebuah instance baru dari kelas [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
| [ArchiveEntrySettings(CompressionSettings compressionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-) | Menginisialisasi sebuah instance baru dari kelas [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
| [ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-) | Menginisialisasi sebuah instance baru dari kelas [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getComment()](#getComment--) | Mendapatkan komentar untuk entri dalam arsip ZIP. |
| [getCompressionSettings()](#getCompressionSettings--) | Mendapatkan pengaturan untuk rutin kompresi atau dekompresi. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Mendapatkan pengaturan untuk enkripsi atau dekripsi. |
| [setComment(String value)](#setComment-java.lang.String-) | Komentar untuk entri dalam arsip ZIP. |
### ArchiveEntrySettings() {#ArchiveEntrySettings--}
```
public ArchiveEntrySettings()
```


Menginisialisasi sebuah instance baru dari kelas [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

### ArchiveEntrySettings(CompressionSettings compressionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings)
```


Menginisialisasi sebuah instance baru dari kelas [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Pengaturan untuk kompresi. Berikan null untuk pengaturan deflate default. |

Dapat menjadi salah satu dari berikut:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |

### ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)
```


Menginisialisasi sebuah instance baru dari kelas [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Pengaturan untuk kompresi. Berikan null untuk pengaturan deflate default. |

Dapat menjadi salah satu dari berikut:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |
|  | encryptionSettings | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | Pengaturan untuk enkripsi. Berikan null jika tidak perlu mengenkripsi atau mendekripsi. |

Dapat menjadi salah satu dari berikut:

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) |

### getComment() {#getComment--}
```
public final String getComment()
```


Mendapatkan komentar untuk entri dalam arsip ZIP.

**Returns:**
java.lang.String - komentar untuk entri dalam arsip ZIP.
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Mendapatkan pengaturan untuk rutin kompresi atau dekompresi.

Dapat menjadi salah satu dari berikut:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings)

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression routine.
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final EncryptionSettings getEncryptionSettings()
```


Mendapatkan pengaturan untuk enkripsi atau dekripsi. Pengaturan untuk entri tertentu dapat berbeda.

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - settings for encryption or decryption. Settings of particular entry may vary.
### setComment(String value) {#setComment-java.lang.String-}
```
public final void setComment(String value)
```


Komentar untuk entri dalam arsip ZIP.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String |  |

