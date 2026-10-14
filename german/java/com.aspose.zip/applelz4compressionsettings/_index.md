---
title: "AppleLz4CompressionSettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen für LZ4-Kompression in einer Apple‑Archive‑Datei (.aar)."
type: docs
weight: 21
url: /de/java/com.aspose.zip/applelz4compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLz4CompressionSettings extends AppleCompressionSettings
```

Einstellungen für die LZ4-Kompression innerhalb einer Apple-Archivdatei (.aar).
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [AppleLz4CompressionSettings(int blockSize)](#AppleLz4CompressionSettings-int-) | Initialisiert eine neue Instanz der [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings)-Klasse. |
| [AppleLz4CompressionSettings()](#AppleLz4CompressionSettings--) | Initialisiert eine neue Instanz der [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings)-Klasse mit Standardparametern. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Ermittelt die Größe jedes komprimierten `pbz4`/`bv41`-Blocks. |
### AppleLz4CompressionSettings(int blockSize) {#AppleLz4CompressionSettings-int-}
```
public AppleLz4CompressionSettings(int blockSize)
```


Initialisiert eine neue Instanz der [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings)-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| blockSize | int | Die Größe jedes komprimierten `pbz4`/`bv41`-Blocks. |

### AppleLz4CompressionSettings() {#AppleLz4CompressionSettings--}
```
public AppleLz4CompressionSettings()
```


Initialisiert eine neue Instanz der [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings)-Klasse mit Standardparametern.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Ermittelt die Größe jedes komprimierten `pbz4`/`bv41`-Blocks.

Wert: Der Standardwert beträgt 4 MiB.

**Returns:**
int - die Größe jedes komprimierten `pbz4`/`bv41`-Blocks.
