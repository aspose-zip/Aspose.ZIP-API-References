---
title: "CabEntrySettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Inställningar som styr hur en CAB-post skrivs."
type: docs
weight: 47
url: /sv/java/com.aspose.zip/cabentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class CabEntrySettings
```

Inställningar som styr hur en CAB-post skrivs.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [CabEntrySettings(CabCompressionSettings compressionSettings)](#CabEntrySettings-com.aspose.zip.CabCompressionSettings-) | Initierar inställningarna med en specifik komprimeringsprofil. |
| [CabEntrySettings()](#CabEntrySettings--) | Initierar inställningarna med standard MSZip-komprimering. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | Hämtar komprimeringskonfigurationen som tillämpas på posten. |
### CabEntrySettings(CabCompressionSettings compressionSettings) {#CabEntrySettings-com.aspose.zip.CabCompressionSettings-}
```
public CabEntrySettings(CabCompressionSettings compressionSettings)
```


Initierar inställningarna med en specifik komprimeringsprofil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | compressionSettings | [CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) | Komprimeringsinställningar att använda. |

Kan vara en av dessa: |

### CabEntrySettings() {#CabEntrySettings--}
```
public CabEntrySettings()
```


Initierar inställningarna med standard MSZip-komprimering.

### getCompressionSettings() {#getCompressionSettings--}
```
public final CabCompressionSettings getCompressionSettings()
```


Hämtar komprimeringskonfigurationen som tillämpas på posten.

Kan vara en av dessa:

 *  

**Returns:**
[CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) - the compression configuration applied to the entry.
