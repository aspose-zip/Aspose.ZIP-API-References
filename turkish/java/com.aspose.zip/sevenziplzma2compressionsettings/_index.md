---
title: "SevenZipLZMA2CompressionSettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "7z arşivi içinde LZMA2 sıkıştırma yöntemi için ayarlar."
type: docs
weight: 114
url: /tr/java/com.aspose.zip/sevenziplzma2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMA2CompressionSettings extends SevenZipCompressionSettings
```

7z arşivi içinde LZMA2 sıkıştırma yöntemi için ayarlar.

LZMA2, sıkıştırılmış LZMA verilerinin ve sıkıştırılmamış verilerin birden çok çalıştırılmasını destekler.

Daha fazla bilgi için: [Lempel\\u2013Ziv\\u2013Markov\_chain\_algorithm][Lempel_u2013Ziv_u2013Markov_chain_algorithm]


[Lempel_u2013Ziv_u2013Markov_chain_algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SevenZipLZMA2CompressionSettings()](#SevenZipLZMA2CompressionSettings--) | 7z arşivindeki LZMA2 sıkıştırma yöntemi için ayarları başlatır. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize)](#SevenZipLZMA2CompressionSettings-int-) | 7z arşivindeki LZMA2 sıkıştırma yöntemi için ayarları başlatır. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)](#SevenZipLZMA2CompressionSettings-int-int-) | 7z arşivindeki LZMA2 sıkıştırma yöntemi için ayarları başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Sıkıştırma iş parçacığı sayısını alır. |
| [getDictionarySize()](#getDictionarySize--) | Sözlük (geçmiş tamponu) boyutu, yakın zamanda işlenen sıkıştırılmamış verinin kaç baytının bellekte tutulduğunu gösterir. |
| [getFastBytes()](#getFastBytes--) | LZMA2 sıkıştırıcısı tarafından kullanılan hızlı baytların kontrol sayısını alır. |
| [getMethod()](#getMethod--) | Sıkıştırma veya açma yöntemini alır. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Sıkıştırma iş parçacığı sayısını ayarlar. |
### SevenZipLZMA2CompressionSettings() {#SevenZipLZMA2CompressionSettings--}
```
public SevenZipLZMA2CompressionSettings()
```


7z arşivindeki LZMA2 sıkıştırma yöntemi için ayarları başlatır.

### SevenZipLZMA2CompressionSettings(int dictionarySize) {#SevenZipLZMA2CompressionSettings-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize)
```


7z arşivindeki LZMA2 sıkıştırma yöntemi için ayarları başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | dictionarySize | int | geçmiş tamponunun boyutu, 4096 ile 1073741824 arasında olmalıdır. |

Sözlük ne kadar büyük olursa, genellikle sıkıştırma oranı o kadar iyi olur - ancak sıkıştırılmamış veriden daha büyük sözlükler RAM'in boşa harcanmasıdır. |

### SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes) {#SevenZipLZMA2CompressionSettings-int-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)
```


7z arşivindeki LZMA2 sıkıştırma yöntemi için ayarları başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | dictionarySize | int | geçmiş tamponunun boyutu, 4096 ile 1073741824 arasında olmalıdır. |

Sözlük ne kadar büyük olursa, genellikle sıkıştırma oranı o kadar iyi olur - ancak sıkıştırılmamış veriden daha büyük sözlükler RAM'in boşa harcanmasıdır. |
| fastBytes | int | LZMA2 sıkıştırıcıları tarafından kullanılan fast byte sayısını kontrol eder. Daha büyük bir fast byte sayısı, sıkıştırma hızından ödün vererek daha iyi bir sıkıştırma oranı sağlayabilir. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Sıkıştırma iş parçacığı sayısını alır. Değer 1'den büyükse, çok iş parçacıklı sıkıştırma kullanılacaktır.

**Returns:**
int - sıkıştırma iş parçacığı sayısı
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Sözlük (geçmiş tamponu) boyutu, yakın zamanda işlenen sıkıştırılmamış verinin kaç baytının bellekte tutulduğunu gösterir.

**Returns:**
int - sözlük (geçmiş tamponu) boyutu
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


LZMA2 sıkıştırıcısı tarafından kullanılan hızlı baytların kontrol sayısını alır.

**Returns:**
int - LZMA2 sıkıştırıcı tarafından kullanılan fast byte kontrol sayısı
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Sıkıştırma veya açma yöntemini alır.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method.
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Sıkıştırma iş parçacığı sayısını ayarlar. Değer 1'den büyükse, çok iş parçacıklı sıkıştırma kullanılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | sıkıştırma iş parçacığı sayısı. |

Bu sayıyı CPU çekirdek sayısından fazla ayarlamayın. |

