---
title: "AppleArchiveEntrySettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "İçinde girişleri oluşturmak için kullanılan ayarlar."
type: docs
weight: 18
url: /tr/java/com.aspose.zip/applearchiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class AppleArchiveEntrySettings
```

Girişlerin içinde oluşturulmak için kullanılan ayarlar [AppleArchive](../../com.aspose.zip/applearchive).
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)](#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-) | Yeni bir [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | Oluşturulan Apple Archive yüküne uygulanan sıkıştırma ayarlarını alır. |
| [getIncludeCrc32Checksum()](#getIncludeCrc32Checksum--) | Oluşturulan dosya girişleri için CRC32 kontrol toplamı alanlarının dahil edilip edilmediğini gösteren bir değeri alır. |
| [setIncludeCrc32Checksum(boolean value)](#setIncludeCrc32Checksum-boolean-) | Oluşturulan dosya girişleri için CRC32 kontrol toplamı alanlarının dahil edilip edilmediğini gösteren bir değeri ayarlar. |
### AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings) {#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-}
```
public AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)
```


Yeni bir [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| compressionSettings | [AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) | Oluşturulan Apple Archive yüküne uygulanan sıkıştırma ayarları. |

### getCompressionSettings() {#getCompressionSettings--}
```
public final AppleCompressionSettings getCompressionSettings()
```


Oluşturulan Apple Archive yüküne uygulanan sıkıştırma ayarlarını alır.

**Returns:**
[AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) - compression settings applied to the composed Apple Archive payload.
### getIncludeCrc32Checksum() {#getIncludeCrc32Checksum--}
```
public final boolean getIncludeCrc32Checksum()
```


Oluşturulan dosya girişleri için CRC32 kontrol toplamı alanlarının dahil edilip edilmediğini gösteren bir değeri alır.

**Returns:**
boolean - oluşturulan dosya girişleri için CRC32 kontrol toplamı alanlarının dahil edilip edilmediğini gösteren bir değer.
### setIncludeCrc32Checksum(boolean value) {#setIncludeCrc32Checksum-boolean-}
```
public final void setIncludeCrc32Checksum(boolean value)
```


Oluşturulan dosya girişleri için CRC32 kontrol toplamı alanlarının dahil edilip edilmediğini gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | oluşturulan dosya girişleri için CRC32 kontrol toplamı alanlarının dahil edilip edilmediğini gösteren bir değer. |

