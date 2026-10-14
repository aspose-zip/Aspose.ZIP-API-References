---
title: "AppleArchiveEntrySettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen, die zum Zusammenstellen von Einträgen innerhalb von . verwendet werden."
type: docs
weight: 18
url: /de/java/com.aspose.zip/applearchiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class AppleArchiveEntrySettings
```

Einstellungen, die zum Zusammenstellen von Einträgen innerhalb von [AppleArchive](../../com.aspose.zip/applearchive) verwendet werden.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)](#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-) | Initialisiert eine neue Instanz der Klasse [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | Ruft die Komprimierungseinstellungen ab, die auf die zusammengesetzte Apple Archive-Payload angewendet werden. |
| [getIncludeCrc32Checksum()](#getIncludeCrc32Checksum--) | Ruft einen Wert ab, der angibt, ob CRC32‑Prüfsummenfelder für zusammengesetzte Dateieinträge enthalten sind. |
| [setIncludeCrc32Checksum(boolean value)](#setIncludeCrc32Checksum-boolean-) | Setzt einen Wert, der angibt, ob CRC32‑Prüfsummenfelder für zusammengesetzte Dateieinträge enthalten sind. |
### AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings) {#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-}
```
public AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)
```


Initialisiert eine neue Instanz der Klasse [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| compressionSettings | [AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) | Komprimierungseinstellungen, die auf die zusammengesetzte Apple Archive-Payload angewendet werden. |

### getCompressionSettings() {#getCompressionSettings--}
```
public final AppleCompressionSettings getCompressionSettings()
```


Ruft die Komprimierungseinstellungen ab, die auf die zusammengesetzte Apple Archive-Payload angewendet werden.

**Returns:**
[AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) - compression settings applied to the composed Apple Archive payload.
### getIncludeCrc32Checksum() {#getIncludeCrc32Checksum--}
```
public final boolean getIncludeCrc32Checksum()
```


Ruft einen Wert ab, der angibt, ob CRC32‑Prüfsummenfelder für zusammengesetzte Dateieinträge enthalten sind.

**Returns:**
boolean – ein Wert, der angibt, ob CRC32‑Prüfsummenfelder für zusammengesetzte Dateieinträge enthalten sind.
### setIncludeCrc32Checksum(boolean value) {#setIncludeCrc32Checksum-boolean-}
```
public final void setIncludeCrc32Checksum(boolean value)
```


Setzt einen Wert, der angibt, ob CRC32‑Prüfsummenfelder für zusammengesetzte Dateieinträge enthalten sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob CRC32‑Prüfsummenfelder für zusammengesetzte Dateieinträge enthalten sind. |

