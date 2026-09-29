---
title: "Bzip2CompressionSettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni per la compressione Bzip2 all'interno di un archivio ZIP."
type: docs
weight: 41
url: /it/java/com.aspose.zip/bzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class Bzip2CompressionSettings extends CompressionSettings
```

Impostazioni per la compressione Bzip2 all'interno di un archivio ZIP.

bzip2 comprime i file utilizzando l'algoritmo di compressione testuale a ordinamento a blocchi Burrows-Wheeler e la codifica Huffman.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Bzip2CompressionSettings(int blockSize)](#Bzip2CompressionSettings-int-) | Inizializza una nuova istanza della classe [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings). |
| [Bzip2CompressionSettings()](#Bzip2CompressionSettings--) | Inizializza una nuova istanza della classe [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) con dimensione di blocco predefinita, pari a 9 centinaia di kilobyte. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Dimensione del blocco in centinaia di kilobyte. |
### Bzip2CompressionSettings(int blockSize) {#Bzip2CompressionSettings-int-}
```
public Bzip2CompressionSettings(int blockSize)
```


Inizializza una nuova istanza della classe [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1)))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | Block size in hundreds of kilobytes. |

### Bzip2CompressionSettings() {#Bzip2CompressionSettings--}
```
public Bzip2CompressionSettings()
```


Initializes a new instance of the [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) class with default block size, equals to 9 hundred of kilobytes.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save(zipFile);
     }
 
```



### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Dimensione del blocco in centinaia di kilobyte.

**Returns:**
int - dimensione del blocco in centinaia di kilobyte
