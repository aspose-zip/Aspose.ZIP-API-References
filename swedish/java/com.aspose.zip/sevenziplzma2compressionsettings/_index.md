---
title: "SevenZipLZMA2CompressionSettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Inställningar för LZMA2-komprimeringsmetod i ett 7z-arkiv."
type: docs
weight: 114
url: /sv/java/com.aspose.zip/sevenziplzma2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMA2CompressionSettings extends SevenZipCompressionSettings
```

Inställningar för LZMA2-komprimeringsmetod i ett 7z-arkiv.

LZMA2 stödjer flera körningar av komprimerad LZMA-data och okomprimerad data.

Se mer: [Lempel\\\\u2013Ziv\\\\u2013Markov\\_chain\\_algorithm][Lempel_u2013Ziv_u2013Markov_chain_algorithm]


[Lempel_u2013Ziv_u2013Markov_chain_algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [SevenZipLZMA2CompressionSettings()](#SevenZipLZMA2CompressionSettings--) | Instansierar inställningar för LZMA2-komprimeringsmetoden i ett 7z-arkiv. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize)](#SevenZipLZMA2CompressionSettings-int-) | Instansierar inställningar för LZMA2-komprimeringsmetoden i ett 7z-arkiv. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)](#SevenZipLZMA2CompressionSettings-int-int-) | Instansierar inställningar för LZMA2-komprimeringsmetoden i ett 7z-arkiv. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Hämtar antalet komprimeringstrådar. |
| [getDictionarySize()](#getDictionarySize--) | Storleken på ordboken (historikbuffert) indikerar hur många byte av den nyligen bearbetade okomprimerade datan som hålls i minnet. |
| [getFastBytes()](#getFastBytes--) | Hämtar kontrollnumret för snabba byte som används av LZMA2-komprimeraren. |
| [getMethod()](#getMethod--) | Hämtar komprimerings- eller dekomprimeringsmetod. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Ställer in antalet komprimeringstrådar. |
### SevenZipLZMA2CompressionSettings() {#SevenZipLZMA2CompressionSettings--}
```
public SevenZipLZMA2CompressionSettings()
```


Instansierar inställningar för LZMA2-komprimeringsmetoden i ett 7z-arkiv.

### SevenZipLZMA2CompressionSettings(int dictionarySize) {#SevenZipLZMA2CompressionSettings-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize)
```


Instansierar inställningar för LZMA2-komprimeringsmetoden i ett 7z-arkiv.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | dictionarySize | int | storleken på historikbufferten, måste vara mellan 4096 och 1073741824. |

Ju större ordboken är, desto bättre är vanligtvis komprimeringsgraden – men ordböcker som är större än den okomprimerade datan är slöseri med RAM. |

### SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes) {#SevenZipLZMA2CompressionSettings-int-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)
```


Instansierar inställningar för LZMA2-komprimeringsmetoden i ett 7z-arkiv.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | dictionarySize | int | storleken på historikbufferten, måste vara mellan 4096 och 1073741824. |

Ju större ordboken är, desto bättre är vanligtvis komprimeringsgraden – men ordböcker som är större än den okomprimerade datan är slöseri med RAM. |
| fastBytes | int | styr antalet snabba byte som används av LZMA2-komprimerarna. Ett större antal snabba byte kan ge en bättre komprimeringsgrad på bekostnad av komprimeringshastigheten. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Hämtar antalet komprimeringstrådar. Om värdet är större än 1 kommer komprimering med flera trådar att användas.

**Returns:**
int - antalet komprimeringstrådar
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Storleken på ordboken (historikbuffert) indikerar hur många byte av den nyligen bearbetade okomprimerade datan som hålls i minnet.

**Returns:**
int – ordbok (historikbuffer) storlek
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


Hämtar kontrollnumret för snabba byte som används av LZMA2-komprimeraren.

**Returns:**
int – kontrollnumret för snabba byte som används av LZMA2-komprimeraren
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Hämtar komprimerings- eller dekomprimeringsmetod.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method.
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Ställer in antalet komprimeringstrådar. Om värdet är större än 1 kommer komprimering med flera trådar att användas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | antalet komprimeringstrådar. |

Ställ inte in detta nummer högre än CPU-kärnor. |

