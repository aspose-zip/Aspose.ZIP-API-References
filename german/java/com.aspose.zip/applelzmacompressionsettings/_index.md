---
title: "AppleLzmaCompressionSettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen für LZMA-Kompression innerhalb einer Apple Archive .aar-Datei."
type: docs
weight: 23
url: /de/java/com.aspose.zip/applelzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLzmaCompressionSettings extends AppleCompressionSettings
```

Einstellungen für die LZMA-Kompression innerhalb einer Apple-Archivdatei (.aar).
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [AppleLzmaCompressionSettings(int blockSize)](#AppleLzmaCompressionSettings-int-) | Initialisiert eine neue Instanz der [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) Klasse. |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize)](#AppleLzmaCompressionSettings-int-int-) | Initialisiert eine neue Instanz der [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) Klasse. |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)](#AppleLzmaCompressionSettings-int-int-int-) | Initialisiert eine neue Instanz der [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) Klasse. |
| [AppleLzmaCompressionSettings()](#AppleLzmaCompressionSettings--) | Initialisiert eine neue Instanz der Klasse [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) mit Standardparametern. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Ermittelt die Größe jedes Datenblocks vor der Komprimierung. |
| [getDictionarySize()](#getDictionarySize--) | Ermittelt die für die Komprimierung verwendete Wörterbuchgröße. |
| [getFastBytes()](#getFastBytes--) | Ermittelt die für die Komprimierung verwendete Anzahl schneller Bytes. |
### AppleLzmaCompressionSettings(int blockSize) {#AppleLzmaCompressionSettings-int-}
```
public AppleLzmaCompressionSettings(int blockSize)
```


Initialisiert eine neue Instanz der [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| blockSize | int | Die Größe jedes Datenblocks vor der Komprimierung. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize) {#AppleLzmaCompressionSettings-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize)
```


Initialisiert eine neue Instanz der [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| blockSize | int | Die Größe jedes Datenblocks vor der Komprimierung. |
| dictionarySize | int | Die für die Komprimierung verwendete Wörterbuchgröße. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes) {#AppleLzmaCompressionSettings-int-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)
```


Initialisiert eine neue Instanz der [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| blockSize | int | Die Größe jedes Datenblocks vor der Komprimierung. |
| dictionarySize | int | Die für die Komprimierung verwendete Wörterbuchgröße. |
| fastBytes | int | Die für die Komprimierung verwendete Anzahl schneller Bytes. |

### AppleLzmaCompressionSettings() {#AppleLzmaCompressionSettings--}
```
public AppleLzmaCompressionSettings()
```


Initialisiert eine neue Instanz der Klasse [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) mit Standardparametern.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Ermittelt die Größe jedes Datenblocks vor der Komprimierung.

Wert: Der Standardwert beträgt 4 MiB.

**Returns:**
int - die Größe jedes Datenblocks vor der Komprimierung.
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Ermittelt die für die Komprimierung verwendete Wörterbuchgröße.

Wert: Der Standardwert ist 8 MiB.

**Returns:**
int - die für die Komprimierung verwendete Wörterbuchgröße.
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


Ermittelt die für die Komprimierung verwendete Anzahl schneller Bytes.

Wert: Der Standardwert ist 32.

**Returns:**
int - die für die Komprimierung verwendete Anzahl schneller Bytes.
