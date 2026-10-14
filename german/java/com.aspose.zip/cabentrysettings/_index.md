---
title: "CabEntrySettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen, die steuern, wie ein CAB-Eintrag geschrieben wird."
type: docs
weight: 47
url: /de/java/com.aspose.zip/cabentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class CabEntrySettings
```

Einstellungen, die steuern, wie ein CAB-Eintrag geschrieben wird.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [CabEntrySettings(CabCompressionSettings compressionSettings)](#CabEntrySettings-com.aspose.zip.CabCompressionSettings-) | Initialisiert die Einstellungen mit einem bestimmten Komprimierungsprofil. |
| [CabEntrySettings()](#CabEntrySettings--) | Initialisiert die Einstellungen mit der Standard-MSZip-Kompression. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | Liefert die auf den Eintrag angewendete Komprimierungskonfiguration. |
### CabEntrySettings(CabCompressionSettings compressionSettings) {#CabEntrySettings-com.aspose.zip.CabCompressionSettings-}
```
public CabEntrySettings(CabCompressionSettings compressionSettings)
```


Initialisiert die Einstellungen mit einem bestimmten Komprimierungsprofil.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | compressionSettings | [CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) | Zu verwendende Komprimierungseinstellungen. |

Kann einer dieser sein: |

### CabEntrySettings() {#CabEntrySettings--}
```
public CabEntrySettings()
```


Initialisiert die Einstellungen mit der Standard-MSZip-Kompression.

### getCompressionSettings() {#getCompressionSettings--}
```
public final CabCompressionSettings getCompressionSettings()
```


Liefert die auf den Eintrag angewendete Komprimierungskonfiguration.

Kann einer der folgenden sein:

 *  

**Returns:**
[CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) - the compression configuration applied to the entry.
