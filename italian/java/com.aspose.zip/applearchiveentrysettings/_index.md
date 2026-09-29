---
title: "AppleArchiveEntrySettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni utilizzate per comporre le voci all'interno di ."
type: docs
weight: 18
url: /it/java/com.aspose.zip/applearchiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class AppleArchiveEntrySettings
```

Impostazioni utilizzate per comporre le voci all'interno di [AppleArchive](../../com.aspose.zip/applearchive).
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)](#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-) | Inizializza una nuova istanza della classe [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | Ottiene le impostazioni di compressione applicate al payload Apple Archive composto. |
| [getIncludeCrc32Checksum()](#getIncludeCrc32Checksum--) | Ottiene un valore che indica se i campi di checksum CRC32 sono inclusi per le voci di file composte. |
| [setIncludeCrc32Checksum(boolean value)](#setIncludeCrc32Checksum-boolean-) | Imposta un valore che indica se i campi di checksum CRC32 sono inclusi per le voci di file composte. |
### AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings) {#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-}
```
public AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)
```


Inizializza una nuova istanza della classe [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| compressionSettings | [AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) | Impostazioni di compressione applicate al payload Apple Archive composto. |

### getCompressionSettings() {#getCompressionSettings--}
```
public final AppleCompressionSettings getCompressionSettings()
```


Ottiene le impostazioni di compressione applicate al payload Apple Archive composto.

**Returns:**
[AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) - compression settings applied to the composed Apple Archive payload.
### getIncludeCrc32Checksum() {#getIncludeCrc32Checksum--}
```
public final boolean getIncludeCrc32Checksum()
```


Ottiene un valore che indica se i campi di checksum CRC32 sono inclusi per le voci di file composte.

**Returns:**
boolean - un valore che indica se i campi di checksum CRC32 sono inclusi per le voci di file composte.
### setIncludeCrc32Checksum(boolean value) {#setIncludeCrc32Checksum-boolean-}
```
public final void setIncludeCrc32Checksum(boolean value)
```


Imposta un valore che indica se i campi di checksum CRC32 sono inclusi per le voci di file composte.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se i campi di checksum CRC32 sono inclusi per le voci di file composte. |

