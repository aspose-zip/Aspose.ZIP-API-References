---
title: "AppleLz4CompressionSettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni per la compressione LZ4 all'interno di un file Apple Archive .aar."
type: docs
weight: 21
url: /it/java/com.aspose.zip/applelz4compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLz4CompressionSettings extends AppleCompressionSettings
```

Impostazioni per la compressione LZ4 all'interno di un file Apple Archive (.aar).
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [AppleLz4CompressionSettings(int blockSize)](#AppleLz4CompressionSettings-int-) | Inizializza una nuova istanza della classe [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings). |
| [AppleLz4CompressionSettings()](#AppleLz4CompressionSettings--) | Inizializza una nuova istanza della classe [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) con parametri predefiniti. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Restituisce la dimensione di ogni blocco compresso `pbz4`/`bv41`. |
### AppleLz4CompressionSettings(int blockSize) {#AppleLz4CompressionSettings-int-}
```
public AppleLz4CompressionSettings(int blockSize)
```


Inizializza una nuova istanza della classe [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| blockSize | int | La dimensione di ogni blocco compresso `pbz4`/`bv41`. |

### AppleLz4CompressionSettings() {#AppleLz4CompressionSettings--}
```
public AppleLz4CompressionSettings()
```


Inizializza una nuova istanza della classe [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) con parametri predefiniti.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Restituisce la dimensione di ogni blocco compresso `pbz4`/`bv41`.

Valore: il valore predefinito è 4 MiB.

**Returns:**
int - la dimensione di ogni blocco compresso `pbz4`/`bv41`.
