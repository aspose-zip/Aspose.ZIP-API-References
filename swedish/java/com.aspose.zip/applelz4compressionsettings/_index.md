---
title: "AppleLz4CompressionSettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Inställningar för LZ4-komprimering i en Apple Archive .aar-fil."
type: docs
weight: 21
url: /sv/java/com.aspose.zip/applelz4compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLz4CompressionSettings extends AppleCompressionSettings
```

Inställningar för LZ4-komprimering i en Apple Archive (.aar)-fil.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [AppleLz4CompressionSettings(int blockSize)](#AppleLz4CompressionSettings-int-) | Initierar en ny instans av klassen [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings). |
| [AppleLz4CompressionSettings()](#AppleLz4CompressionSettings--) | Initierar en ny instans av klassen [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) med standardparametrar. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Hämtar storleken på varje komprimerat `pbz4`/`bv41`-block. |
### AppleLz4CompressionSettings(int blockSize) {#AppleLz4CompressionSettings-int-}
```
public AppleLz4CompressionSettings(int blockSize)
```


Initierar en ny instans av klassen [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| blockSize | int | Storleken på varje komprimerat `pbz4`/`bv41`-block. |

### AppleLz4CompressionSettings() {#AppleLz4CompressionSettings--}
```
public AppleLz4CompressionSettings()
```


Initierar en ny instans av klassen [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) med standardparametrar.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Hämtar storleken på varje komprimerat `pbz4`/`bv41`-block.

Värde: Standardvärdet är 4 MiB.

**Returns:**
int - storleken på varje komprimerat `pbz4`/`bv41`-block.
