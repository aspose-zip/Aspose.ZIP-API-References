---
title: "LzmaArchiveSettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Lzma arşivi için ayarlar."
type: docs
weight: 87
url: /tr/java/com.aspose.zip/lzmaarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzmaArchiveSettings
```

Lzma arşivi için ayarlar.

Lempel‑Ziv‑Markov zinciri algoritması (LZMA), kayıpsız veri sıkıştırması yapmak için kullanılan bir algoritmadır. Bu algoritma, LZ77 algoritmasına benzer bir sözlük sıkıştırma şeması kullanır ve yüksek sıkıştırma oranı ile değişken bir sıkıştırma‑sözlük boyutu sunar.

Daha fazla bilgi için: [Lempel\u2013Ziv\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [LzmaArchiveSettings()](#LzmaArchiveSettings--) | Varsayılan sözlük boyutu 16 megabayt, hızlı bayt sayısı 32 ve literal bağlam bitleri 3 olan yeni bir [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | Ham akışın bir bölümü sıkıştırıldığında tetiklenen bir olayı alır. |
| [getDictionarySize()](#getDictionarySize--) | Sözlük (geçmiş tamponu) boyutu, yakın zamanda işlenen sıkıştırılmamış verinin kaç baytının bellekte tutulduğunu gösterir. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Literal bağlam bitlerinin sayısını alır. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | LZMA algoritmasında hızlı eşleşme araması için kullanılan bayt sayısını alır. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Ham akışın bir bölümü sıkıştırıldığında tetiklenen bir olayı ayarlar. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | Sözlük (geçmiş tamponu) boyutu, yakın zamanda işlenen sıkıştırılmamış verinin kaç baytının bellekte tutulduğunu gösterir. |
| [setLiteralContextBits(int value)](#setLiteralContextBits-int-) | Literal bağlam bitlerinin sayısını ayarlar. |
| [setNumberOfFastBytes(int value)](#setNumberOfFastBytes-int-) | LZMA algoritmasında hızlı eşleşme araması için kullanılan bayt sayısını ayarlar. |
### LzmaArchiveSettings() {#LzmaArchiveSettings--}
```
public LzmaArchiveSettings()
```


Varsayılan sözlük boyutu 16 megabayt, hızlı bayt sayısı 32 ve literal bağlam bitleri 3 olan yeni bir [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) sınıfı örneği başlatır.

```

``````

LzmaArchiveSettings settings = new LzmaArchiveSettings();
settings.setDictionarySize(1048576);
try (LzmaArchive archive = new LzmaArchive(settings)) {
archive.setSource(\"data.bin\");
archive.save(lzmaFile);
}
 
```



### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Gets an event that is raised when a portion of raw stream compressed.

```

``````

    lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```



**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Dictionary (history buffer) size, yakın zamanda işlenen sıkıştırılmamış verinin kaç baytının bellekte tutulduğunu gösterir. Ayarlanmamışsa, giriş boyutuna göre seçilir.

Sözlük ne kadar büyük olursa, genellikle sıkıştırma oranı o kadar iyi olur - ancak sıkıştırılmamış veriden daha büyük sözlükler RAM israfıdır. LZMA arşivinin sözlük boyutu ya iki üssü (2^n) ya da iki üssünün üç katı (3\\*2^n) olmalıdır.

**Returns:**
int - Dictionary (history buffer) size.
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


Literal bağlam bitlerinin sayısını alır.

Literal Context Bits, önceki sıkıştırılmamış baytin en anlamlı bitlerinden kaç tanesinin sonraki literal baytin bitlerini tahmin etmek için kullanıldığını tanımlar. 0 ile 8 arasında olmalıdır.

**Returns:**
int - literal context bit sayısı.
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


LZMA algoritmasında hızlı eşleşme araması için kullanılan bayt sayısını alır.

Daha yüksek bir değer, sıkıştırıcının daha uzun eşleşmeler aramasına izin verir; bu, sıkıştırma oranını hafifçe artırabilir ancak sıkıştırma hızını yavaşlatır.

**Returns:**
int - LZMA algoritmasında hızlı eşleşme araması için kullanılan bayt sayısı.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Ham akışın bir bölümü sıkıştırıldığında tetiklenen bir olayı ayarlar.

```

``````

lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when a portion of raw stream compressed |

### setDictionarySize(int value) {#setDictionarySize-int-}
```
public final void setDictionarySize(int value)
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory. If not set, will be chosen accordingly to entry size.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM. The disctionary size of LZMA archive must be either a power of two (2^n) or three times a power of two (3\*2^n).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | Dictionary (history buffer) size. |

### setLiteralContextBits(int value) {#setLiteralContextBits-int-}
```
public final void setLiteralContextBits(int value)
```


Sets the number of literal context bits.

Literal Context Bits define how many of the most significant bits of the previous uncompressed byte are used to predict the bits of the next literal byte. Must be from 0 to 8.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of literal context bits. |

### setNumberOfFastBytes(int value) {#setNumberOfFastBytes-int-}
```
public final void setNumberOfFastBytes(int value)
```


Sets the number of bytes used for fast match searching in the LZMA algorithm.

A higher value allows the compressor to search longer matches, which can improve the compression ratio slightly but slows down compression.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of bytes used for fast match searching in the LZMA algorithm. |

