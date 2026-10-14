---
title: "SevenZipBZip2CompressionSettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen voor BZip2-compressiemethode binnen een 7z-archief."
type: docs
weight: 109
url: /nl/java/com.aspose.zip/sevenzipbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipBZip2CompressionSettings extends SevenZipCompressionSettings
```

Instellingen voor BZip2-compressiemethode binnen een 7z-archief.

Bzip2 comprimeert bestanden met behulp van het Burrows-Wheeler bloksorteringstekstcompressie-algoritme en Huffman-codering.

Zie meer: [Bzip2][]


[Bzip2]: https://en.wikipedia.org/wiki/Bzip2
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [SevenZipBZip2CompressionSettings(int blockSize)](#SevenZipBZip2CompressionSettings-int-) | Initialiseert een nieuw exemplaar van de klasse [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings). |
| [SevenZipBZip2CompressionSettings()](#SevenZipBZip2CompressionSettings--) | Initialiseert een nieuw exemplaar van de klasse [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) met de standaard blokgrootte, gelijk aan 9 honderd kilobytes. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Blokgrootte in honderden kilobytes. |
| [getMethod()](#getMethod--) | Haalt compressie- of decompressiemethode op. |
### SevenZipBZip2CompressionSettings(int blockSize) {#SevenZipBZip2CompressionSettings-int-}
```
public SevenZipBZip2CompressionSettings(int blockSize)
```


Initialiseert een nieuw exemplaar van de klasse [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| blockSize | int | blokgrootte in honderden kilobytes |

### SevenZipBZip2CompressionSettings() {#SevenZipBZip2CompressionSettings--}
```
public SevenZipBZip2CompressionSettings()
```


Initialiseert een nieuw exemplaar van de klasse [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) met de standaard blokgrootte, gelijk aan 9 honderd kilobytes.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Blokgrootte in honderden kilobytes.

**Returns:**
int - blokgrootte in honderden kilobytes
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Haalt compressie- of decompressiemethode op.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
