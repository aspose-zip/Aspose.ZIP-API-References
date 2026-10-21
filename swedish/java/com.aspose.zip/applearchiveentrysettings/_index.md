---
title: "AppleArchiveEntrySettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Inställningar som används för att komponera poster i ."
type: docs
weight: 18
url: /sv/java/com.aspose.zip/applearchiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class AppleArchiveEntrySettings
```

Inställningar som används för att komponera poster i [AppleArchive](../../com.aspose.zip/applearchive).
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)](#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-) | Initierar en ny instans av klassen [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | Hämtar komprimeringsinställningarna som tillämpas på den sammansatta Apple Archive-payloaden. |
| [getIncludeCrc32Checksum()](#getIncludeCrc32Checksum--) | Hämtar ett värde som indikerar om CRC32-kontrollsummefält är inkluderade för sammansatta filposter. |
| [setIncludeCrc32Checksum(boolean value)](#setIncludeCrc32Checksum-boolean-) | Ställer in ett värde som indikerar om CRC32-kontrollsummefält är inkluderade för sammansatta filposter. |
### AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings) {#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-}
```
public AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)
```


Initierar en ny instans av klassen [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| compressionSettings | [AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) | Komprimeringsinställningar som tillämpas på den sammansatta Apple Archive-payloaden. |

### getCompressionSettings() {#getCompressionSettings--}
```
public final AppleCompressionSettings getCompressionSettings()
```


Hämtar komprimeringsinställningarna som tillämpas på den sammansatta Apple Archive-payloaden.

**Returns:**
[AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) - compression settings applied to the composed Apple Archive payload.
### getIncludeCrc32Checksum() {#getIncludeCrc32Checksum--}
```
public final boolean getIncludeCrc32Checksum()
```


Hämtar ett värde som indikerar om CRC32-kontrollsummefält är inkluderade för sammansatta filposter.

**Returns:**
boolean - ett värde som indikerar om CRC32-kontrollsummefält är inkluderade för sammansatta filposter.
### setIncludeCrc32Checksum(boolean value) {#setIncludeCrc32Checksum-boolean-}
```
public final void setIncludeCrc32Checksum(boolean value)
```


Ställer in ett värde som indikerar om CRC32-kontrollsummefält är inkluderade för sammansatta filposter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om CRC32-kontrollsummefält är inkluderade för sammansatta filposter. |

