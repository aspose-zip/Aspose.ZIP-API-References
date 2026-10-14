---
title: "AppleLzmaCompressionSettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni per la compressione LZMA all'interno di un file Apple Archive .aar."
type: docs
weight: 23
url: /it/java/com.aspose.zip/applelzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLzmaCompressionSettings extends AppleCompressionSettings
```

Impostazioni per la compressione LZMA all'interno di un file Apple Archive (.aar).
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [AppleLzmaCompressionSettings(int blockSize)](#AppleLzmaCompressionSettings-int-) | Inizializza una nuova istanza della classe [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize)](#AppleLzmaCompressionSettings-int-int-) | Inizializza una nuova istanza della classe [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)](#AppleLzmaCompressionSettings-int-int-int-) | Inizializza una nuova istanza della classe [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings()](#AppleLzmaCompressionSettings--) | Inizializza una nuova istanza della classe [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) con i parametri predefiniti. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Ottiene la dimensione di ciascun blocco di dati prima della compressione. |
| [getDictionarySize()](#getDictionarySize--) | Ottiene la dimensione del dizionario utilizzata per la compressione. |
| [getFastBytes()](#getFastBytes--) | Ottiene il numero di byte rapidi utilizzati per la compressione. |
### AppleLzmaCompressionSettings(int blockSize) {#AppleLzmaCompressionSettings-int-}
```
public AppleLzmaCompressionSettings(int blockSize)
```


Inizializza una nuova istanza della classe [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| blockSize | int | La dimensione di ciascun blocco di dati prima della compressione. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize) {#AppleLzmaCompressionSettings-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize)
```


Inizializza una nuova istanza della classe [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| blockSize | int | La dimensione di ciascun blocco di dati prima della compressione. |
| dictionarySize | int | La dimensione del dizionario utilizzata per la compressione. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes) {#AppleLzmaCompressionSettings-int-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)
```


Inizializza una nuova istanza della classe [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| blockSize | int | La dimensione di ciascun blocco di dati prima della compressione. |
| dictionarySize | int | La dimensione del dizionario utilizzata per la compressione. |
| fastBytes | int | Il numero di byte rapidi utilizzati per la compressione. |

### AppleLzmaCompressionSettings() {#AppleLzmaCompressionSettings--}
```
public AppleLzmaCompressionSettings()
```


Inizializza una nuova istanza della classe [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) con i parametri predefiniti.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Ottiene la dimensione di ciascun blocco di dati prima della compressione.

Valore: il valore predefinito è 4 MiB.

**Returns:**
int - la dimensione di ciascun blocco di dati prima della compressione.
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Ottiene la dimensione del dizionario utilizzata per la compressione.

Valore: il valore predefinito è 8 MiB.

**Returns:**
int - la dimensione del dizionario utilizzata per la compressione.
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


Ottiene il numero di byte rapidi utilizzati per la compressione.

Valore: il valore predefinito è 32.

**Returns:**
int - il numero di byte rapidi utilizzati per la compressione.
