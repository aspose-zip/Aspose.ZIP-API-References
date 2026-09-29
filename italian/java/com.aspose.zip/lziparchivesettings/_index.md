---
title: "LzipArchiveSettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "La classe contiene le impostazioni di un particolare archivio lzip."
type: docs
weight: 84
url: /it/java/com.aspose.zip/lziparchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzipArchiveSettings
```

La classe contiene le impostazioni di un particolare archivio lzip.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [LzipArchiveSettings(int dictionarySize)](#LzipArchiveSettings-int-) | Inizializza una nuova istanza di [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con una dimensione del dizionario specifica. |
| [LzipArchiveSettings(int dictionarySize, int maxMemberSize)](#LzipArchiveSettings-int-int-) | Inizializza una nuova istanza di [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con una dimensione del dizionario specifica. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Restituisce il conteggio dei thread di compressione. |
| [getDictionarySize()](#getDictionarySize--) | Restituisce la dimensione del dizionario utilizzato dalla compressione LZMA. |
| [getFastSpeed()](#getFastSpeed--) | Restituisce l'istanza della classe [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con dimensione del dizionario pari a 1 megabyte nel filtro LZMA. |
| [getFastestSpeed()](#getFastestSpeed--) | Restituisce l'istanza della classe [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con dimensione del dizionario pari a 65536 byte nel filtro LZMA. |
| [getHighCompression()](#getHighCompression--) | Restituisce l'istanza della classe [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con dimensione del dizionario pari a 32 megabyte nel filtro LZMA. |
| [getMaxMemberSize()](#getMaxMemberSize--) | Restituisce la dimensione massima di un membro nell'archivio lzip, espressa in byte. |
| [getMaximumCompression()](#getMaximumCompression--) | Restituisce l'istanza della classe [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con dimensione del dizionario pari a 64 megabyte nel filtro LZMA. |
| [getNormal()](#getNormal--) | Restituisce l'istanza della classe [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con dimensione del dizionario pari a 16 megabyte nel filtro LZMA. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Imposta il conteggio dei thread di compressione. |
### LzipArchiveSettings(int dictionarySize) {#LzipArchiveSettings-int-}
```
public LzipArchiveSettings(int dictionarySize)
```


Inizializza una nuova istanza di [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con una dimensione del dizionario specifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dictionarySize | int | dimensione del dizionario per la compressione LZMA in byte |

### LzipArchiveSettings(int dictionarySize, int maxMemberSize) {#LzipArchiveSettings-int-int-}
```
public LzipArchiveSettings(int dictionarySize, int maxMemberSize)
```


Inizializza una nuova istanza di [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con una dimensione del dizionario specifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dictionarySize | int | dimensione del dizionario per la compressione LZMA in byte |
| maxMemberSize | int | Dimensione massima di un membro nell'archivio lzip, espressa in byte. Il valore predefinito è 60 MB. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Restituisce il numero di thread di compressione. Se il valore è maggiore di 1, verrà utilizzata la compressione multithread.

**Returns:**
int - numero di thread di compressione
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Restituisce la dimensione del dizionario utilizzato dalla compressione LZMA.

**Returns:**
int - dimensione del dizionario utilizzato dalla compressione LZMA
### getFastSpeed() {#getFastSpeed--}
```
public static LzipArchiveSettings getFastSpeed()
```


Restituisce l'istanza della classe [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con dimensione del dizionario pari a 1 megabyte nel filtro LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 1 megabyte in LZMA filter
### getFastestSpeed() {#getFastestSpeed--}
```
public static LzipArchiveSettings getFastestSpeed()
```


Restituisce l'istanza della classe [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con dimensione del dizionario pari a 65536 byte nel filtro LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 65536 bytes in LZMA filter
### getHighCompression() {#getHighCompression--}
```
public static LzipArchiveSettings getHighCompression()
```


Restituisce l'istanza della classe [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con dimensione del dizionario pari a 32 megabyte nel filtro LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 32 megabytes in LZMA filter
### getMaxMemberSize() {#getMaxMemberSize--}
```
public final long getMaxMemberSize()
```


Restituisce la dimensione massima di un membro nell'archivio lzip, espressa in byte.

**Returns:**
long - dimensione massima di un membro nell'archivio lzip, espressa in byte
### getMaximumCompression() {#getMaximumCompression--}
```
public static LzipArchiveSettings getMaximumCompression()
```


Restituisce l'istanza della classe [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con dimensione del dizionario pari a 64 megabyte nel filtro LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 64 megabytes in LZMA filter
### getNormal() {#getNormal--}
```
public static LzipArchiveSettings getNormal()
```


Restituisce l'istanza della classe [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con dimensione del dizionario pari a 16 megabyte nel filtro LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 16 megabytes in LZMA filter
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Imposta il conteggio dei thread di compressione. Se il valore è maggiore di 1, verrà utilizzata la compressione multithread.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | conteggio dei thread di compressione |

