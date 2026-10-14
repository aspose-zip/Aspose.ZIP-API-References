---
title: "SevenZipLZMA2CompressionSettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen voor LZMA2-compressiemethode binnen een 7z-archief."
type: docs
weight: 114
url: /nl/java/com.aspose.zip/sevenziplzma2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMA2CompressionSettings extends SevenZipCompressionSettings
```

Instellingen voor LZMA2-compressiemethode binnen een 7z-archief.

LZMA2 ondersteunt meerdere runs van gecomprimeerde LZMA-gegevens en ongecomprimeerde gegevens.

See more: [Lempel\\u2013Ziv\\u2013Markov\_chain\_algorithm][Lempel_u2013Ziv_u2013Markov_chain_algorithm]


[Lempel_u2013Ziv_u2013Markov_chain_algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [SevenZipLZMA2CompressionSettings()](#SevenZipLZMA2CompressionSettings--) | Instantieert instellingen voor de LZMA2-compressiemethode binnen een 7z-archief. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize)](#SevenZipLZMA2CompressionSettings-int-) | Instantieert instellingen voor de LZMA2-compressiemethode binnen een 7z-archief. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)](#SevenZipLZMA2CompressionSettings-int-int-) | Instantieert instellingen voor de LZMA2-compressiemethode binnen een 7z-archief. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Haalt het aantal compressiedraden op. |
| [getDictionarySize()](#getDictionarySize--) | De grootte van het woordenboek (geschiedenisbuffer) geeft aan hoeveel bytes van de recent verwerkte ongecomprimeerde gegevens in het geheugen worden bewaard. |
| [getFastBytes()](#getFastBytes--) | Haalt het controlegetal van snelle bytes op dat door de LZMA2-compressor wordt gebruikt. |
| [getMethod()](#getMethod--) | Haalt compressie- of decompressiemethode op. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Stelt het aantal compressiedraden in. |
### SevenZipLZMA2CompressionSettings() {#SevenZipLZMA2CompressionSettings--}
```
public SevenZipLZMA2CompressionSettings()
```


Instantieert instellingen voor de LZMA2-compressiemethode binnen een 7z-archief.

### SevenZipLZMA2CompressionSettings(int dictionarySize) {#SevenZipLZMA2CompressionSettings-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize)
```


Instantieert instellingen voor de LZMA2-compressiemethode binnen een 7z-archief.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | dictionarySize | int | de grootte van de geschiedenisbuffer, moet tussen 4096 en 1073741824 liggen. |

Hoe groter het woordenboek, hoe beter de compressieverhouding meestal is - maar woordenboeken die groter zijn dan de ongecomprimeerde data zijn een verspilling van RAM. |

### SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes) {#SevenZipLZMA2CompressionSettings-int-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)
```


Instantieert instellingen voor de LZMA2-compressiemethode binnen een 7z-archief.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | dictionarySize | int | de grootte van de geschiedenisbuffer, moet tussen 4096 en 1073741824 liggen. |

Hoe groter het woordenboek, hoe beter de compressieverhouding meestal is - maar woordenboeken die groter zijn dan de ongecomprimeerde data zijn een verspilling van RAM. |
| fastBytes | int | bepaalt het aantal snelle bytes dat door de LZMA2-compressors wordt gebruikt. Een groter aantal snelle bytes kan een betere compressieverhouding opleveren ten koste van de compressiesnelheid. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Haalt het aantal compressiedraden op. Als de waarde groter is dan 1, wordt multithread-compressie gebruikt.

**Returns:**
int - aantal compressiedraden
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


De grootte van het woordenboek (geschiedenisbuffer) geeft aan hoeveel bytes van de recent verwerkte ongecomprimeerde gegevens in het geheugen worden bewaard.

**Returns:**
int - woordenboek (geschiedenisbuffer) grootte
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


Haalt het controlegetal van snelle bytes op dat door de LZMA2-compressor wordt gebruikt.

**Returns:**
int - het controlegetal van snelle bytes dat door de LZMA2-compressor wordt gebruikt
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Haalt compressie- of decompressiemethode op.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method.
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Stelt het aantal compressiedraden in. Als de waarde groter is dan 1, wordt multithread-compressie gebruikt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | aantal compressiedraden. |

Stel dit getal niet hoger in dan het aantal CPU-kernen. |

