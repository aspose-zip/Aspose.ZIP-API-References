---
title: "CabEntrySettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni che controllano come viene scritto un elemento CAB."
type: docs
weight: 47
url: /it/java/com.aspose.zip/cabentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class CabEntrySettings
```

Impostazioni che controllano come viene scritto un elemento CAB.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [CabEntrySettings(CabCompressionSettings compressionSettings)](#CabEntrySettings-com.aspose.zip.CabCompressionSettings-) | Inizializza le impostazioni con un profilo di compressione specifico. |
| [CabEntrySettings()](#CabEntrySettings--) | Inizializza le impostazioni con la compressione MSZip predefinita. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | Ottiene la configurazione di compressione applicata all'elemento. |
### CabEntrySettings(CabCompressionSettings compressionSettings) {#CabEntrySettings-com.aspose.zip.CabCompressionSettings-}
```
public CabEntrySettings(CabCompressionSettings compressionSettings)
```


Inizializza le impostazioni con un profilo di compressione specifico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | compressionSettings | [CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) | Impostazioni di compressione da utilizzare. |

Può essere uno di questi: |

### CabEntrySettings() {#CabEntrySettings--}
```
public CabEntrySettings()
```


Inizializza le impostazioni con la compressione MSZip predefinita.

### getCompressionSettings() {#getCompressionSettings--}
```
public final CabCompressionSettings getCompressionSettings()
```


Ottiene la configurazione di compressione applicata all'elemento.

Può essere uno di questi:

 *  

**Returns:**
[CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) - the compression configuration applied to the entry.
