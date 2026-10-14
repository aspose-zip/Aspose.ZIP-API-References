---
title: "CabEntrySettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen die bepalen hoe een CAB-item wordt geschreven."
type: docs
weight: 47
url: /nl/java/com.aspose.zip/cabentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class CabEntrySettings
```

Instellingen die bepalen hoe een CAB-item wordt geschreven.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [CabEntrySettings(CabCompressionSettings compressionSettings)](#CabEntrySettings-com.aspose.zip.CabCompressionSettings-) | Initialiseert instellingen met een specifiek compressieprofiel. |
| [CabEntrySettings()](#CabEntrySettings--) | Initialiseert instellingen met standaard MSZip-compressie. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | Haalt de compressieconfiguratie op die op het item wordt toegepast. |
### CabEntrySettings(CabCompressionSettings compressionSettings) {#CabEntrySettings-com.aspose.zip.CabCompressionSettings-}
```
public CabEntrySettings(CabCompressionSettings compressionSettings)
```


Initialiseert instellingen met een specifiek compressieprofiel.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | compressionSettings | [CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) | Compressie-instellingen om te gebruiken. |

Kan een van deze zijn: |

### CabEntrySettings() {#CabEntrySettings--}
```
public CabEntrySettings()
```


Initialiseert instellingen met standaard MSZip-compressie.

### getCompressionSettings() {#getCompressionSettings--}
```
public final CabCompressionSettings getCompressionSettings()
```


Haalt de compressieconfiguratie op die op het item wordt toegepast.

Kan een van deze zijn:

 *  

**Returns:**
[CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) - the compression configuration applied to the entry.
