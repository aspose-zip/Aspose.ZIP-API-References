---
title: "SevenZipBZip2CompressionSettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "7z arşivi içinde BZip2 sıkıştırma yöntemi için ayarlar."
type: docs
weight: 109
url: /tr/java/com.aspose.zip/sevenzipbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipBZip2CompressionSettings extends SevenZipCompressionSettings
```

7z arşivi içinde BZip2 sıkıştırma yöntemi için ayarlar.

Bzip2, dosyaları Burrows-Wheeler blok sıralama metin sıkıştırma algoritması ve Huffman kodlaması kullanarak sıkıştırır.

Daha fazla: [Bzip2][]


[Bzip2]: https://en.wikipedia.org/wiki/Bzip2
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SevenZipBZip2CompressionSettings(int blockSize)](#SevenZipBZip2CompressionSettings-int-) | Yeni bir [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) sınıfı örneği başlatır. |
| [SevenZipBZip2CompressionSettings()](#SevenZipBZip2CompressionSettings--) | Varsayılan blok boyutu 9 yüz kilobayt olan yeni bir [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Blok boyutu yüz kilobyte cinsinden. |
| [getMethod()](#getMethod--) | Sıkıştırma veya açma yöntemini alır. |
### SevenZipBZip2CompressionSettings(int blockSize) {#SevenZipBZip2CompressionSettings-int-}
```
public SevenZipBZip2CompressionSettings(int blockSize)
```


Yeni bir [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| blockSize | int | blok boyutu yüz kilobayt cinsinden |

### SevenZipBZip2CompressionSettings() {#SevenZipBZip2CompressionSettings--}
```
public SevenZipBZip2CompressionSettings()
```


Varsayılan blok boyutu 9 yüz kilobayt olan yeni bir [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) sınıfı örneği başlatır.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Blok boyutu yüz kilobyte cinsinden.

**Returns:**
int - blok boyutu yüz kilobyte cinsinden
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Sıkıştırma veya açma yöntemini alır.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
