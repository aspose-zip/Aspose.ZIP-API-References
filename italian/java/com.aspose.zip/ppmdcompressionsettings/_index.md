---
title: "PPMdCompressionSettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni per la compressione PPMd all'interno di un archivio ZIP."
type: docs
weight: 93
url: /it/java/com.aspose.zip/ppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class PPMdCompressionSettings extends CompressionSettings
```

Impostazioni per la compressione PPMd all'interno di un archivio ZIP.

PPMd è un algoritmo di compressione dati sviluppato da Dmitry Shkarin. Questo algoritmo si basa sul matching predittivo di frasi su contesti di ordine multiplo.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [PPMdCompressionSettings(int modelOrder, int suballocatorSize)](#PPMdCompressionSettings-int-int-) | Inizializza una nuova istanza della classe [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings). |
| [PPMdCompressionSettings()](#PPMdCompressionSettings--) | Inizializza una nuova istanza della classe [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) con ordine modello predefinito e dimensione del sub-allocatore. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getModelOrder()](#getModelOrder--) | Restituisce l'ordine del modello. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Restituisce la dimensione del sub-allocatore in MB. |
### PPMdCompressionSettings(int modelOrder, int suballocatorSize) {#PPMdCompressionSettings-int-int-}
```
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```


Inizializza una nuova istanza della classe [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10)))) {
archive.createEntry("data.bin", "data.bin");
archive.save("zipFile.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| modelOrder | int | Order of the model.

Bigger model orders almost surely results in better compression and surely more memory and CPU usage. |
| suballocatorSize | int | Memory size in MB suballocator may consume.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse. |

### PPMdCompressionSettings() {#PPMdCompressionSettings--}
```
public PPMdCompressionSettings()
```


Initializes a new instance of the [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) class with default model order and sub-allocator size.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("zipFile.zip");
     }
 
```

L'ordine modello predefinito è 8 e la dimensione del sub-allocatore è 50 MB.

### getModelOrder() {#getModelOrder--}
```
public final int getModelOrder()
```


Restituisce l'ordine del modello.

**Returns:**
int - l'ordine del modello
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Restituisce la dimensione del sub-allocatore in MB.

**Returns:**
int - la dimensione del sub-allocatore in MB
