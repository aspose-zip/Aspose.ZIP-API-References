---
title: "SevenZipEntrySettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan yang digunakan untuk mengompresi atau mendekompresi entri 7z."
type: docs
weight: 113
url: /id/java/com.aspose.zip/sevenzipentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipEntrySettings
```

Pengaturan yang digunakan untuk mengompresi atau mendekompresi entri 7z.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [SevenZipEntrySettings()](#SevenZipEntrySettings--) | Menginisialisasi instance baru dari kelas [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-) | Menginisialisasi instance baru dari kelas [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-) | Menginisialisasi instance baru dari kelas [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getCompressHeader()](#getCompressHeader--) | Mendapatkan nilai yang menunjukkan apakah header arsip akan dikompres. |
| [getCompressionSettings()](#getCompressionSettings--) | Mendapatkan pengaturan untuk rutin kompresi atau dekompresi. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Mendapatkan pengaturan untuk enkripsi atau dekripsi. |
| [getSolid()](#getSolid--) | Mendapatkan nilai yang menunjukkan apakah entri akan digabungkan dan diperlakukan sebagai satu blok data. |
| [setCompressHeader(boolean value)](#setCompressHeader-boolean-) | Mengatur nilai yang menunjukkan apakah header arsip akan dikompres. |
| [setSolid(boolean value)](#setSolid-boolean-) | Mengatur nilai yang menunjukkan apakah entri akan digabungkan dan diperlakukan sebagai satu blok data. |
### SevenZipEntrySettings() {#SevenZipEntrySettings--}
```
public SevenZipEntrySettings()
```


Menginisialisasi instance baru dari kelas [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)
```


Menginisialisasi instance baru dari kelas [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | pengaturan untuk kompresi. Berikan null untuk pengaturan LZMA default. |

Dapat menjadi salah satu dari berikut:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)
```


Menginisialisasi instance baru dari kelas [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | pengaturan untuk kompresi. Berikan null untuk pengaturan LZMA default. |

Dapat menjadi salah satu dari berikut:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |
|  | encryptionSettings | [SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) | pengaturan untuk enkripsi. Berikan null jika tidak perlu mengenkripsi atau mendekripsi. |

Hanya dapat satu:

 *  [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) |

### getCompressHeader() {#getCompressHeader--}
```
public final boolean getCompressHeader()
```


Mendapatkan nilai yang menunjukkan apakah header arsip akan dikompres.

Pengaturan ini setara dengan saklar `-mhc=on` pada alat 7-Zip. Saat ini, tidak kompatibel dengan enkripsi header.

**Returns:**
boolean - nilai yang menunjukkan apakah header arsip akan dikompres
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


Mendapatkan pengaturan untuk rutin kompresi atau dekompresi.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression routine
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final SevenZipEncryptionSettings getEncryptionSettings()
```


Mendapatkan pengaturan untuk enkripsi atau dekripsi. Pengaturan untuk entri tertentu dapat berbeda.

The [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) adalah satu-satunya opsi untuk arsip 7z.

**Returns:**
[SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) - settings for encryption or decryption
### getSolid() {#getSolid--}
```
public final boolean getSolid()
```


Mendapatkan nilai yang menunjukkan apakah entri akan digabungkan dan diperlakukan sebagai satu blok data.

Contoh berikut menunjukkan cara mengompres direktori menjadi arsip 7z solid dengan kompresi LZMA2 tanpa enkripsi.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
SevenZipEntrySettings settings = new SevenZipEntrySettings(new SevenZipLZMACompressionSettings());
settings.setSolid(true);
try (SevenZipArchive archive = new SevenZipArchive(settings)) {
archive.createEntries("C:\\Documents");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

Provide `SevenZipEntrySettings` for solid 7z archive on archive instantiation.

**Returns:**
boolean - value indicating whether to concatenate entries and treat them as a single data block.
### setCompressHeader(boolean value) {#setCompressHeader-boolean-}
```
public final void setCompressHeader(boolean value)
```


Sets value indicating whether to compress archive header.

This setting is equivalent `-mhc=on` switch of 7-Zip tool. Currently, it is incompatible with header encryption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to compress archive header |

### setSolid(boolean value) {#setSolid-boolean-}
```
public final void setSolid(boolean value)
```


Sets value indicating whether to concatenate entries and treat them as a single data block.

The following example shows how to compress a directory to solid 7z archive with LZMA2 compression without encryption.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         SevenZipEntrySettings settings = new SevenZipEntrySettings(new SevenZipLZMACompressionSettings());
         settings.setSolid(true);
         try (SevenZipArchive archive = new SevenZipArchive(settings)) {
             archive.createEntries("C:\\Documents");
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

Sediakan `SevenZipEntrySettings` untuk arsip 7z solid pada saat pembuatan arsip.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah entri akan digabungkan dan diperlakukan sebagai satu blok data. |

