---
title: "SevenZipLZMA2CompressionSettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen für die LZMA2-Kompressionsmethode innerhalb eines 7z-Archivs."
type: docs
weight: 114
url: /de/java/com.aspose.zip/sevenziplzma2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMA2CompressionSettings extends SevenZipCompressionSettings
```

Einstellungen für die LZMA2-Kompressionsmethode innerhalb eines 7z-Archivs.

LZMA2 unterstützt mehrere Durchläufe komprimierter LZMA-Daten und unkomprimierter Daten.

Siehe mehr: [Lempel\\u2013Ziv\\u2013Markov\_chain\_algorithm][Lempel_u2013Ziv_u2013Markov_chain_algorithm]


[Lempel_u2013Ziv_u2013Markov_chain_algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SevenZipLZMA2CompressionSettings()](#SevenZipLZMA2CompressionSettings--) | Instanziiert Einstellungen für die LZMA2-Komprimierungsmethode innerhalb eines 7z-Archivs. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize)](#SevenZipLZMA2CompressionSettings-int-) | Instanziiert Einstellungen für die LZMA2-Komprimierungsmethode innerhalb eines 7z-Archivs. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)](#SevenZipLZMA2CompressionSettings-int-int-) | Instanziiert Einstellungen für die LZMA2-Komprimierungsmethode innerhalb eines 7z-Archivs. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Liefert die Anzahl der Komprimierungs-Threads. |
| [getDictionarySize()](#getDictionarySize--) | Die Größe des Wörterbuchs (History‑Puffer) gibt an, wie viele Bytes der zuletzt verarbeiteten unkomprimierten Daten im Speicher gehalten werden. |
| [getFastBytes()](#getFastBytes--) | Ermittelt die Steuerungszahl der schnellen Bytes, die vom LZMA2-Kompressor verwendet werden. |
| [getMethod()](#getMethod--) | Liefert die Komprimierungs- oder Dekomprimierungsmethode. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Setzt die Anzahl der Komprimierungs-Threads. |
### SevenZipLZMA2CompressionSettings() {#SevenZipLZMA2CompressionSettings--}
```
public SevenZipLZMA2CompressionSettings()
```


Instanziiert Einstellungen für die LZMA2-Komprimierungsmethode innerhalb eines 7z-Archivs.

### SevenZipLZMA2CompressionSettings(int dictionarySize) {#SevenZipLZMA2CompressionSettings-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize)
```


Instanziiert Einstellungen für die LZMA2-Komprimierungsmethode innerhalb eines 7z-Archivs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | dictionarySize | int | Die Größe des Verlaufs-Puffers muss zwischen 4096 und 1073741824 liegen. |

Je größer das Wörterbuch, desto besser ist in der Regel das Kompressionsverhältnis – aber Wörterbücher, die größer als die unkomprimierten Daten sind, verschwenden RAM. |

### SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes) {#SevenZipLZMA2CompressionSettings-int-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)
```


Instanziiert Einstellungen für die LZMA2-Komprimierungsmethode innerhalb eines 7z-Archivs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | dictionarySize | int | Die Größe des Verlaufs-Puffers muss zwischen 4096 und 1073741824 liegen. |

Je größer das Wörterbuch, desto besser ist in der Regel das Kompressionsverhältnis – aber Wörterbücher, die größer als die unkomprimierten Daten sind, verschwenden RAM. |
| fastBytes | int | Steuert die Anzahl der schnellen Bytes, die von den LZMA2-Kompressoren verwendet werden. Eine größere Anzahl schneller Bytes kann ein besseres Kompressionsverhältnis bieten, jedoch auf Kosten der Kompressionsgeschwindigkeit. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Gibt die Anzahl der Kompressionsthreads zurück. Wenn der Wert größer als 1 ist, wird eine Multithread-Kompression verwendet.

**Returns:**
int - Anzahl der Kompressionsthreads
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Die Größe des Wörterbuchs (History‑Puffer) gibt an, wie viele Bytes der zuletzt verarbeiteten unkomprimierten Daten im Speicher gehalten werden.

**Returns:**
int – Wörterbuch (Verlaufs-Puffer) Größe
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


Ermittelt die Steuerungszahl der schnellen Bytes, die vom LZMA2-Kompressor verwendet werden.

**Returns:**
int – die Steuerungszahl der schnellen Bytes, die vom LZMA2-Kompressor verwendet werden
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Liefert die Komprimierungs- oder Dekomprimierungsmethode.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method.
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Setzt die Anzahl der Komprimierungs-Threads. Wenn der Wert größer als 1 ist, wird eine mehrthreadige Komprimierung verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Komprimierungs-Thread-Anzahl. |

Setzen Sie diese Zahl nicht höher als die CPU-Kerne. |

