---
title: "CabEntrySettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres qui contrôlent la façon dont une entrée CAB est écrite."
type: docs
weight: 47
url: /fr/java/com.aspose.zip/cabentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class CabEntrySettings
```

Paramètres qui contrôlent la façon dont une entrée CAB est écrite.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [CabEntrySettings(CabCompressionSettings compressionSettings)](#CabEntrySettings-com.aspose.zip.CabCompressionSettings-) | Initialise les paramètres avec un profil de compression spécifique. |
| [CabEntrySettings()](#CabEntrySettings--) | Initialise les paramètres avec la compression MSZip par défaut. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | Obtient la configuration de compression appliquée à l'entrée. |
### CabEntrySettings(CabCompressionSettings compressionSettings) {#CabEntrySettings-com.aspose.zip.CabCompressionSettings-}
```
public CabEntrySettings(CabCompressionSettings compressionSettings)
```


Initialise les paramètres avec un profil de compression spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | compressionSettings | [CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) | Paramètres de compression à utiliser. |

Peut être l'un de ceux-ci : |

### CabEntrySettings() {#CabEntrySettings--}
```
public CabEntrySettings()
```


Initialise les paramètres avec la compression MSZip par défaut.

### getCompressionSettings() {#getCompressionSettings--}
```
public final CabCompressionSettings getCompressionSettings()
```


Obtient la configuration de compression appliquée à l'entrée.

Peut être l'un de ceux-ci :

 *  

**Returns:**
[CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) - the compression configuration applied to the entry.
