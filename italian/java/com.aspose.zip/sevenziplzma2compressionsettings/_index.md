---
title: "SevenZipLZMA2CompressionSettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni per il metodo di compressione LZMA2 all'interno di un archivio 7z."
type: docs
weight: 114
url: /it/java/com.aspose.zip/sevenziplzma2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMA2CompressionSettings extends SevenZipCompressionSettings
```

Impostazioni per il metodo di compressione LZMA2 all'interno di un archivio 7z.

LZMA2 supporta più esecuzioni di dati LZMA compressi e dati non compressi.

Vedi di più: [Lempel\\u2013Ziv\\u2013Markov\_chain\_algorithm][Lempel_u2013Ziv_u2013Markov_chain_algorithm]


[Lempel_u2013Ziv_u2013Markov_chain_algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SevenZipLZMA2CompressionSettings()](#SevenZipLZMA2CompressionSettings--) | Istanzia le impostazioni per il metodo di compressione LZMA2 all'interno dell'archivio 7z. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize)](#SevenZipLZMA2CompressionSettings-int-) | Istanzia le impostazioni per il metodo di compressione LZMA2 all'interno dell'archivio 7z. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)](#SevenZipLZMA2CompressionSettings-int-int-) | Istanzia le impostazioni per il metodo di compressione LZMA2 all'interno dell'archivio 7z. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Restituisce il conteggio dei thread di compressione. |
| [getDictionarySize()](#getDictionarySize--) | La dimensione del dizionario (buffer di cronologia) indica quanti byte dei dati non compressi elaborati di recente sono conservati in memoria. |
| [getFastBytes()](#getFastBytes--) | Ottiene il numero di controllo dei byte rapidi usati dal compressore LZMA2. |
| [getMethod()](#getMethod--) | Ottiene il metodo di compressione o decompressione. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Imposta il conteggio dei thread di compressione. |
### SevenZipLZMA2CompressionSettings() {#SevenZipLZMA2CompressionSettings--}
```
public SevenZipLZMA2CompressionSettings()
```


Istanzia le impostazioni per il metodo di compressione LZMA2 all'interno dell'archivio 7z.

### SevenZipLZMA2CompressionSettings(int dictionarySize) {#SevenZipLZMA2CompressionSettings-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize)
```


Istanzia le impostazioni per il metodo di compressione LZMA2 all'interno dell'archivio 7z.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | dictionarySize | int | la dimensione del buffer di cronologia, deve essere compresa tra 4096 e 1073741824. |

Più grande è il dizionario, di solito migliore è il rapporto di compressione - ma i dizionari più grandi dei dati non compressi sono uno spreco di RAM. |

### SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes) {#SevenZipLZMA2CompressionSettings-int-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)
```


Istanzia le impostazioni per il metodo di compressione LZMA2 all'interno dell'archivio 7z.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | dictionarySize | int | la dimensione del buffer di cronologia, deve essere compresa tra 4096 e 1073741824. |

Più grande è il dizionario, di solito migliore è il rapporto di compressione - ma i dizionari più grandi dei dati non compressi sono uno spreco di RAM. |
| fastBytes | int | controlla il numero di byte rapidi usati dai compressori LZMA2. Un numero maggiore di byte rapidi può fornire un rapporto di compressione migliore a scapito della velocità di compressione. |

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


La dimensione del dizionario (buffer di cronologia) indica quanti byte dei dati non compressi elaborati di recente sono conservati in memoria.

**Returns:**
int - dimensione del dizionario (buffer di cronologia)
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


Ottiene il numero di controllo dei byte rapidi usati dal compressore LZMA2.

**Returns:**
int - il numero di controllo dei byte rapidi usati dal compressore LZMA2
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Ottiene il metodo di compressione o decompressione.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method.
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Imposta il conteggio dei thread di compressione. Se il valore è maggiore di 1, verrà utilizzata la compressione multithread.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | conteggio dei thread di compressione. |

Non impostare questo numero superiore al numero di core CPU. |

