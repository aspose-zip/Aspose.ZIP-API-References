---
title: "SevenZipBZip2CompressionSettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni per il metodo di compressione BZip2 all'interno di un archivio 7z."
type: docs
weight: 109
url: /it/java/com.aspose.zip/sevenzipbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipBZip2CompressionSettings extends SevenZipCompressionSettings
```

Impostazioni per il metodo di compressione BZip2 all'interno di un archivio 7z.

Bzip2 comprime i file utilizzando l'algoritmo di compressione testuale a ordinamento a blocchi Burrows-Wheeler e la codifica Huffman.

Vedi di più: [Bzip2][]


[Bzip2]: https://en.wikipedia.org/wiki/Bzip2
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SevenZipBZip2CompressionSettings(int blockSize)](#SevenZipBZip2CompressionSettings-int-) | Inizializza una nuova istanza della classe [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings). |
| [SevenZipBZip2CompressionSettings()](#SevenZipBZip2CompressionSettings--) | Inizializza una nuova istanza della classe [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) con dimensione di blocco predefinita, pari a 9 centinaia di kilobyte. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Dimensione del blocco in centinaia di kilobyte. |
| [getMethod()](#getMethod--) | Ottiene il metodo di compressione o decompressione. |
### SevenZipBZip2CompressionSettings(int blockSize) {#SevenZipBZip2CompressionSettings-int-}
```
public SevenZipBZip2CompressionSettings(int blockSize)
```


Inizializza una nuova istanza della classe [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| blockSize | int | dimensione del blocco in centinaia di kilobyte |

### SevenZipBZip2CompressionSettings() {#SevenZipBZip2CompressionSettings--}
```
public SevenZipBZip2CompressionSettings()
```


Inizializza una nuova istanza della classe [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) con dimensione di blocco predefinita, pari a 9 centinaia di kilobyte.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Dimensione del blocco in centinaia di kilobyte.

**Returns:**
int - dimensione del blocco in centinaia di kilobyte
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Ottiene il metodo di compressione o decompressione.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
