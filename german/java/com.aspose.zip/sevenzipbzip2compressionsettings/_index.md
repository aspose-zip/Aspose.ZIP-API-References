---
title: "SevenZipBZip2CompressionSettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen für die BZip2-Kompressionsmethode innerhalb eines 7z-Archivs."
type: docs
weight: 109
url: /de/java/com.aspose.zip/sevenzipbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipBZip2CompressionSettings extends SevenZipCompressionSettings
```

Einstellungen für die BZip2-Kompressionsmethode innerhalb eines 7z-Archivs.

Bzip2 komprimiert Dateien mit dem Burrows-Wheeler-Blocksortier-Textkompressionsalgorithmus und Huffman-Codierung.

Mehr dazu: [Bzip2][]


[Bzip2]: https://en.wikipedia.org/wiki/Bzip2
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SevenZipBZip2CompressionSettings(int blockSize)](#SevenZipBZip2CompressionSettings-int-) | Initialisiert eine neue Instanz der Klasse [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings). |
| [SevenZipBZip2CompressionSettings()](#SevenZipBZip2CompressionSettings--) | Initialisiert eine neue Instanz der Klasse [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) mit der Standard-Blockgröße von 9 Hundert Kilobyte. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Blockgröße in Hunderten von Kilobyte. |
| [getMethod()](#getMethod--) | Liefert die Komprimierungs- oder Dekomprimierungsmethode. |
### SevenZipBZip2CompressionSettings(int blockSize) {#SevenZipBZip2CompressionSettings-int-}
```
public SevenZipBZip2CompressionSettings(int blockSize)
```


Initialisiert eine neue Instanz der Klasse [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| blockSize | int | Blockgröße in Hunderten von Kilobyte |

### SevenZipBZip2CompressionSettings() {#SevenZipBZip2CompressionSettings--}
```
public SevenZipBZip2CompressionSettings()
```


Initialisiert eine neue Instanz der Klasse [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) mit der Standard-Blockgröße von 9 Hundert Kilobyte.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Blockgröße in Hunderten von Kilobyte.

**Returns:**
int - Blockgröße in Hunderten von Kilobyte
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Liefert die Komprimierungs- oder Dekomprimierungsmethode.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
