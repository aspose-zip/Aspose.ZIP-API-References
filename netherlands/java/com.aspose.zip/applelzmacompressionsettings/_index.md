---
title: "AppleLzmaCompressionSettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen voor LZMA-compressie binnen een Apple Archive .aar-bestand."
type: docs
weight: 23
url: /nl/java/com.aspose.zip/applelzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLzmaCompressionSettings extends AppleCompressionSettings
```

Instellingen voor LZMA-compressie binnen een Apple Archive (.aar)-bestand.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [AppleLzmaCompressionSettings(int blockSize)](#AppleLzmaCompressionSettings-int-) | Initialiseert een nieuwe instantie van de [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) klasse. |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize)](#AppleLzmaCompressionSettings-int-int-) | Initialiseert een nieuwe instantie van de [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) klasse. |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)](#AppleLzmaCompressionSettings-int-int-int-) | Initialiseert een nieuwe instantie van de [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) klasse. |
| [AppleLzmaCompressionSettings()](#AppleLzmaCompressionSettings--) | Initialiseert een nieuw exemplaar van de [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) klasse met standaardparameters. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Haalt de grootte van elk gegevensblok op vóór compressie. |
| [getDictionarySize()](#getDictionarySize--) | Haalt de grootte van het woordenboek op dat wordt gebruikt voor compressie. |
| [getFastBytes()](#getFastBytes--) | Haalt het aantal snelle bytes op dat wordt gebruikt voor compressie. |
### AppleLzmaCompressionSettings(int blockSize) {#AppleLzmaCompressionSettings-int-}
```
public AppleLzmaCompressionSettings(int blockSize)
```


Initialiseert een nieuwe instantie van de [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| blockSize | int | De grootte van elk gegevensblok vóór compressie. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize) {#AppleLzmaCompressionSettings-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize)
```


Initialiseert een nieuwe instantie van de [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| blockSize | int | De grootte van elk gegevensblok vóór compressie. |
| dictionarySize | int | De grootte van het woordenboek dat wordt gebruikt voor compressie. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes) {#AppleLzmaCompressionSettings-int-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)
```


Initialiseert een nieuwe instantie van de [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| blockSize | int | De grootte van elk gegevensblok vóór compressie. |
| dictionarySize | int | De grootte van het woordenboek dat wordt gebruikt voor compressie. |
| fastBytes | int | Het aantal snelle bytes dat wordt gebruikt voor compressie. |

### AppleLzmaCompressionSettings() {#AppleLzmaCompressionSettings--}
```
public AppleLzmaCompressionSettings()
```


Initialiseert een nieuw exemplaar van de [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) klasse met standaardparameters.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Haalt de grootte van elk gegevensblok op vóór compressie.

Waarde: de standaardwaarde is 4 MiB.

**Returns:**
int - de grootte van elk gegevensblok vóór compressie.
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Haalt de grootte van het woordenboek op dat wordt gebruikt voor compressie.

Waarde: De standaardwaarde is 8 MiB.

**Returns:**
int - de grootte van het woordenboek dat wordt gebruikt voor compressie.
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


Haalt het aantal snelle bytes op dat wordt gebruikt voor compressie.

Waarde: De standaardwaarde is 32.

**Returns:**
int - het aantal snelle bytes dat wordt gebruikt voor compressie.
