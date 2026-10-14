---
title: "SevenZipEntrySettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "7z girdilerini sıkıştırmak veya açmak için kullanılan ayarlar."
type: docs
weight: 113
url: /tr/java/com.aspose.zip/sevenzipentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipEntrySettings
```

7z girdilerini sıkıştırmak veya açmak için kullanılan ayarlar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SevenZipEntrySettings()](#SevenZipEntrySettings--) | Yeni bir [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) sınıfı örneği başlatır. |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-) | Yeni bir [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) sınıfı örneği başlatır. |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-) | Yeni bir [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCompressHeader()](#getCompressHeader--) | Arşiv başlığını sıkıştırıp sıkıştırmayacağını gösteren değeri alır. |
| [getCompressionSettings()](#getCompressionSettings--) | Sıkıştırma veya açma rutinine ait ayarları alır. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Şifreleme veya şifre çözme ayarlarını alır. |
| [getSolid()](#getSolid--) | Girdileri birleştirip tek bir veri bloğu olarak ele alıp almayacağını gösteren değeri alır. |
| [setCompressHeader(boolean value)](#setCompressHeader-boolean-) | Arşiv başlığını sıkıştırıp sıkıştırmayacağını gösteren değeri ayarlar. |
| [setSolid(boolean value)](#setSolid-boolean-) | Girdileri birleştirip tek bir veri bloğu olarak ele alıp almayacağını gösteren değeri ayarlar. |
### SevenZipEntrySettings() {#SevenZipEntrySettings--}
```
public SevenZipEntrySettings()
```


Yeni bir [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) sınıfı örneği başlatır.

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)
```


Yeni bir [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | Sıkıştırma ayarları. Varsayılan LZMA ayarları için null geçirin. |

Bunlardan biri olabilir:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)
```


Yeni bir [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | Sıkıştırma ayarları. Varsayılan LZMA ayarları için null geçirin. |

Bunlardan biri olabilir:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |
|  | encryptionSettings | [SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) | Şifreleme ayarları. Şifreleme veya şifre çözme gerekmediğinde null geçirin. |

Sadece biri olabilir:

 *  [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) |

### getCompressHeader() {#getCompressHeader--}
```
public final boolean getCompressHeader()
```


Arşiv başlığını sıkıştırıp sıkıştırmayacağını gösteren değeri alır.

Bu ayar, 7-Zip aracının `-mhc=on` anahtarına eşdeğerdir. Şu anda, başlık şifrelemesiyle uyumsuzdur.

**Returns:**
boolean - arşiv başlığını sıkıştırıp sıkıştırmayacağını gösteren değer
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


Sıkıştırma veya açma rutinine ait ayarları alır.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression routine
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final SevenZipEncryptionSettings getEncryptionSettings()
```


Şifreleme veya şifre çözme ayarlarını alır. Belirli bir girdinin ayarları değişebilir.

Bu [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings), 7z arşivleri için tek seçenektir.

**Returns:**
[SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) - settings for encryption or decryption
### getSolid() {#getSolid--}
```
public final boolean getSolid()
```


Girdileri birleştirip tek bir veri bloğu olarak ele alıp almayacağını gösteren değeri alır.

Aşağıdaki örnek, bir dizini LZMA2 sıkıştırmasıyla şifreleme olmadan katı 7z arşivine nasıl sıkıştıracağınızı gösterir.

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

Arşiv örneklemesi sırasında katı 7z arşivi için `SevenZipEntrySettings` sağlayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | girişleri birleştirip tek bir veri bloğu olarak ele alıp almayacağını gösteren değer. |

