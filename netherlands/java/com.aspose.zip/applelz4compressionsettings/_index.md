---
title: "AppleLz4CompressionSettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen voor LZ4-compressie binnen een Apple‑Archive‑bestand (.aar)."
type: docs
weight: 21
url: /nl/java/com.aspose.zip/applelz4compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLz4CompressionSettings extends AppleCompressionSettings
```

Instellingen voor LZ4-compressie binnen een Apple Archive (.aar)-bestand.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [AppleLz4CompressionSettings(int blockSize)](#AppleLz4CompressionSettings-int-) | Initialiseert een nieuw exemplaar van de klasse [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings). |
| [AppleLz4CompressionSettings()](#AppleLz4CompressionSettings--) | Initialiseert een nieuw exemplaar van de klasse [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) met standaardparameters. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Haalt de grootte op van elk gecomprimeerd `pbz4`/`bv41`‑blok. |
### AppleLz4CompressionSettings(int blockSize) {#AppleLz4CompressionSettings-int-}
```
public AppleLz4CompressionSettings(int blockSize)
```


Initialiseert een nieuw exemplaar van de klasse [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| blockSize | int | De grootte van elk gecomprimeerd `pbz4`/`bv41`‑blok. |

### AppleLz4CompressionSettings() {#AppleLz4CompressionSettings--}
```
public AppleLz4CompressionSettings()
```


Initialiseert een nieuw exemplaar van de klasse [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) met standaardparameters.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Haalt de grootte op van elk gecomprimeerd `pbz4`/`bv41`‑blok.

Waarde: de standaardwaarde is 4 MiB.

**Returns:**
int - de grootte van elk gecomprimeerd `pbz4`/`bv41`‑blok.
