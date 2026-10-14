---
title: "AppleLz4CompressionSettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: ".aar uzantılı Apple Arşivi içinde LZ4 sıkıştırması için ayarlar."
type: docs
weight: 21
url: /tr/java/com.aspose.zip/applelz4compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLz4CompressionSettings extends AppleCompressionSettings
```

Bir Apple Archive (.aar) dosyasında LZ4 sıkıştırması için ayarlar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [AppleLz4CompressionSettings(int blockSize)](#AppleLz4CompressionSettings-int-) | Yeni bir [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) sınıfı örneği başlatır. |
| [AppleLz4CompressionSettings()](#AppleLz4CompressionSettings--) | Yeni bir [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) sınıfı örneğini varsayılan parametrelerle başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Her sıkıştırılmış `pbz4`/`bv41` bloğunun boyutunu alır. |
### AppleLz4CompressionSettings(int blockSize) {#AppleLz4CompressionSettings-int-}
```
public AppleLz4CompressionSettings(int blockSize)
```


Yeni bir [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| blockSize | int | Her sıkıştırılmış `pbz4`/`bv41` bloğunun boyutu. |

### AppleLz4CompressionSettings() {#AppleLz4CompressionSettings--}
```
public AppleLz4CompressionSettings()
```


Yeni bir [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) sınıfı örneğini varsayılan parametrelerle başlatır.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Her sıkıştırılmış `pbz4`/`bv41` bloğunun boyutunu alır.

Değer: Varsayılan değer 4 MiB'dir.

**Returns:**
int - her sıkıştırılmış `pbz4`/`bv41` bloğunun boyutu.
