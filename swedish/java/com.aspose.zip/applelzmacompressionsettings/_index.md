---
title: "AppleLzmaCompressionSettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Inställningar för LZMA-komprimering i en Apple Archive‑fil (.aar)."
type: docs
weight: 23
url: /sv/java/com.aspose.zip/applelzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLzmaCompressionSettings extends AppleCompressionSettings
```

Inställningar för LZMA-komprimering i en Apple Archive (.aar)-fil.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [AppleLzmaCompressionSettings(int blockSize)](#AppleLzmaCompressionSettings-int-) | Initierar en ny instans av klassen [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize)](#AppleLzmaCompressionSettings-int-int-) | Initierar en ny instans av klassen [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)](#AppleLzmaCompressionSettings-int-int-int-) | Initierar en ny instans av klassen [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings()](#AppleLzmaCompressionSettings--) | Initierar en ny instans av klassen [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) med standardparametrar. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Hämtar storleken på varje datablok innan komprimering. |
| [getDictionarySize()](#getDictionarySize--) | Hämtar ordboksstorleken som används för komprimering. |
| [getFastBytes()](#getFastBytes--) | Hämtar antalet snabba byte som används för komprimering. |
### AppleLzmaCompressionSettings(int blockSize) {#AppleLzmaCompressionSettings-int-}
```
public AppleLzmaCompressionSettings(int blockSize)
```


Initierar en ny instans av klassen [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| blockSize | int | Storleken på varje datablok innan komprimering. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize) {#AppleLzmaCompressionSettings-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize)
```


Initierar en ny instans av klassen [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| blockSize | int | Storleken på varje datablok innan komprimering. |
| dictionarySize | int | Ordboksstorleken som används för komprimering. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes) {#AppleLzmaCompressionSettings-int-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)
```


Initierar en ny instans av klassen [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| blockSize | int | Storleken på varje datablok innan komprimering. |
| dictionarySize | int | Ordboksstorleken som används för komprimering. |
| fastBytes | int | Antalet snabba byte som används för komprimering. |

### AppleLzmaCompressionSettings() {#AppleLzmaCompressionSettings--}
```
public AppleLzmaCompressionSettings()
```


Initierar en ny instans av klassen [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) med standardparametrar.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Hämtar storleken på varje datablok innan komprimering.

Värde: Standardvärdet är 4 MiB.

**Returns:**
int - storleken på varje datablok innan komprimering.
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Hämtar ordboksstorleken som används för komprimering.

Värde: Standardvärdet är 8 MiB.

**Returns:**
int - ordboksstorleken som används för komprimering.
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


Hämtar antalet snabba byte som används för komprimering.

Värde: Standardvärdet är 32.

**Returns:**
int - antalet snabba byte som används för komprimering.
