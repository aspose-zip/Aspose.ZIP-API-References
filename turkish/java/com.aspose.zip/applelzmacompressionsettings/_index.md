---
title: "AppleLzmaCompressionSettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Apple Arşivi .aar dosyası içinde LZMA sıkıştırması için ayarlar."
type: docs
weight: 23
url: /tr/java/com.aspose.zip/applelzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLzmaCompressionSettings extends AppleCompressionSettings
```

Bir Apple Archive (.aar) dosyasında LZMA sıkıştırması için ayarlar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [AppleLzmaCompressionSettings(int blockSize)](#AppleLzmaCompressionSettings-int-) | Yeni bir [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) sınıfı örneği başlatır. |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize)](#AppleLzmaCompressionSettings-int-int-) | Yeni bir [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) sınıfı örneği başlatır. |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)](#AppleLzmaCompressionSettings-int-int-int-) | Yeni bir [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) sınıfı örneği başlatır. |
| [AppleLzmaCompressionSettings()](#AppleLzmaCompressionSettings--) | Varsayılan parametrelerle yeni bir [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Sıkıştırmadan önce her veri bloğunun boyutunu alır. |
| [getDictionarySize()](#getDictionarySize--) | Sıkıştırma için kullanılan sözlük boyutunu alır. |
| [getFastBytes()](#getFastBytes--) | Sıkıştırma için kullanılan hızlı bayt sayısını alır. |
### AppleLzmaCompressionSettings(int blockSize) {#AppleLzmaCompressionSettings-int-}
```
public AppleLzmaCompressionSettings(int blockSize)
```


Yeni bir [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| blockSize | int | Sıkıştırmadan önce her veri bloğunun boyutu. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize) {#AppleLzmaCompressionSettings-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize)
```


Yeni bir [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| blockSize | int | Sıkıştırmadan önce her veri bloğunun boyutu. |
| dictionarySize | int | Sıkıştırma için kullanılan sözlük boyutu. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes) {#AppleLzmaCompressionSettings-int-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)
```


Yeni bir [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| blockSize | int | Sıkıştırmadan önce her veri bloğunun boyutu. |
| dictionarySize | int | Sıkıştırma için kullanılan sözlük boyutu. |
| fastBytes | int | Sıkıştırma için kullanılan hızlı bayt sayısı. |

### AppleLzmaCompressionSettings() {#AppleLzmaCompressionSettings--}
```
public AppleLzmaCompressionSettings()
```


Varsayılan parametrelerle yeni bir [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) sınıfı örneği başlatır.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Sıkıştırmadan önce her veri bloğunun boyutunu alır.

Değer: Varsayılan değer 4 MiB'dir.

**Returns:**
int - sıkıştırmadan önce her veri bloğunun boyutu.
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Sıkıştırma için kullanılan sözlük boyutunu alır.

Değer: Varsayılan değer 8 MiB'dir.

**Returns:**
int - sıkıştırma için kullanılan sözlük boyutu.
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


Sıkıştırma için kullanılan hızlı bayt sayısını alır.

Değer: Varsayılan değer 32'dir.

**Returns:**
int - sıkıştırma için kullanılan hızlı bayt sayısı.
