---
title: "Lz4ArchiveSetting"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni per la composizione dell'archivio LZ4."
type: docs
weight: 81
url: /it/java/com.aspose.zip/lz4archivesetting/
---

**Inheritance:**
java.lang.Object
```
public class Lz4ArchiveSetting
```

Impostazioni per la composizione dell'archivio LZ4.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Lz4ArchiveSetting()](#Lz4ArchiveSetting--) | Inizializza una nuova istanza di [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) con parametri predefiniti. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getIncludeBlockChecksum()](#getIncludeBlockChecksum--) | Restituisce un valore che indica se includere l'hash xxh32 compresso alla fine del blocco compresso. |
| [getIncludeContentChecksum()](#getIncludeContentChecksum--) | Restituisce un valore che indica se includere l'hash xxh32 del contenuto alla fine dell'archivio LZ4. |
| [getIncludeContentSize()](#getIncludeContentSize--) | Restituisce un valore che indica se includere la dimensione del contenuto nel frame. |
| [setIncludeBlockChecksum(boolean value)](#setIncludeBlockChecksum-boolean-) | Imposta un valore che indica se includere l'hash xxh32 compresso alla fine del blocco compresso. |
| [setIncludeContentChecksum(boolean value)](#setIncludeContentChecksum-boolean-) | Imposta un valore che indica se includere l'hash xxh32 del contenuto alla fine dell'archivio LZ4. |
| [setIncludeContentSize(boolean value)](#setIncludeContentSize-boolean-) | Imposta un valore che indica se includere la dimensione del contenuto nel frame. |
### Lz4ArchiveSetting() {#Lz4ArchiveSetting--}
```
public Lz4ArchiveSetting()
```


Inizializza una nuova istanza di [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) con parametri predefiniti.

### getIncludeBlockChecksum() {#getIncludeBlockChecksum--}
```
public final boolean getIncludeBlockChecksum()
```


Restituisce un valore che indica se includere l'hash xxh32 compresso alla fine del blocco compresso.

Il valore predefinito è false.

**Returns:**
boolean - un valore che indica se includere l'hash xxh32 compresso alla fine del blocco compresso.
### getIncludeContentChecksum() {#getIncludeContentChecksum--}
```
public final boolean getIncludeContentChecksum()
```


Restituisce un valore che indica se includere l'hash xxh32 del contenuto alla fine dell'archivio LZ4.

Il valore predefinito è true.

**Returns:**
boolean - un valore che indica se includere l'hash xxh32 del contenuto alla fine dell'archivio LZ4.
### getIncludeContentSize() {#getIncludeContentSize--}
```
public final boolean getIncludeContentSize()
```


Restituisce un valore che indica se includere la dimensione del contenuto nel frame.

Il valore predefinito è false. Applicato quando lo stream di origine è ricercabile.

**Returns:**
boolean - un valore che indica se includere la dimensione del contenuto nel frame.
### setIncludeBlockChecksum(boolean value) {#setIncludeBlockChecksum-boolean-}
```
public final void setIncludeBlockChecksum(boolean value)
```


Imposta un valore che indica se includere l'hash xxh32 compresso alla fine del blocco compresso.

Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se includere l'hash xxh32 compresso alla fine del blocco compresso. |

### setIncludeContentChecksum(boolean value) {#setIncludeContentChecksum-boolean-}
```
public final void setIncludeContentChecksum(boolean value)
```


Imposta un valore che indica se includere l'hash xxh32 del contenuto alla fine dell'archivio LZ4.

Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se includere l'hash xxh32 del contenuto alla fine dell'archivio LZ4. |

### setIncludeContentSize(boolean value) {#setIncludeContentSize-boolean-}
```
public final void setIncludeContentSize(boolean value)
```


Imposta un valore che indica se includere la dimensione del contenuto nel frame.

Il valore predefinito è false. Applicato quando lo stream di origine è ricercabile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se includere la dimensione del contenuto nel frame. |

