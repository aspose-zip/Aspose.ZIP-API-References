---
title: "SevenZipBZip2CompressionSettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Inställningar för BZip2-komprimeringsmetod i ett 7z-arkiv."
type: docs
weight: 109
url: /sv/java/com.aspose.zip/sevenzipbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipBZip2CompressionSettings extends SevenZipCompressionSettings
```

Inställningar för BZip2-komprimeringsmetod i ett 7z-arkiv.

Bzip2 komprimerar filer med Burrows-Wheeler blocksorteringsalgoritmen för textkomprimering och Huffman-kodning.

Se mer: [Bzip2][]


[Bzip2]: https://en.wikipedia.org/wiki/Bzip2
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [SevenZipBZip2CompressionSettings(int blockSize)](#SevenZipBZip2CompressionSettings-int-) | Initierar en ny instans av klassen [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings). |
| [SevenZipBZip2CompressionSettings()](#SevenZipBZip2CompressionSettings--) | Initierar en ny instans av klassen [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) med standardblockstorlek, motsvarande 9 hundra kilobyte. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Blockstorlek i hundra kilobyte. |
| [getMethod()](#getMethod--) | Hämtar komprimerings- eller dekomprimeringsmetod. |
### SevenZipBZip2CompressionSettings(int blockSize) {#SevenZipBZip2CompressionSettings-int-}
```
public SevenZipBZip2CompressionSettings(int blockSize)
```


Initierar en ny instans av klassen [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| blockSize | int | blockstorlek i hundra kilobyte |

### SevenZipBZip2CompressionSettings() {#SevenZipBZip2CompressionSettings--}
```
public SevenZipBZip2CompressionSettings()
```


Initierar en ny instans av klassen [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) med standardblockstorlek, motsvarande 9 hundra kilobyte.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Blockstorlek i hundra kilobyte.

**Returns:**
int - blockstorlek i hundra kilobyte
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Hämtar komprimerings- eller dekomprimeringsmetod.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
