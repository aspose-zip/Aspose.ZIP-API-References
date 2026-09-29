---
title: "SevenZipPPMdCompressionSettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni per il metodo di compressione PPMd all'interno di un archivio 7z."
type: docs
weight: 117
url: /it/java/com.aspose.zip/sevenzipppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public final class SevenZipPPMdCompressionSettings extends SevenZipCompressionSettings
```

Impostazioni per il metodo di compressione PPMd all'interno di un archivio 7z.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)](#SevenZipPPMdCompressionSettings-int-int-) | Istanzia le impostazioni per il metodo di compressione PPMd all'interno di un archivio 7z. |
| [SevenZipPPMdCompressionSettings()](#SevenZipPPMdCompressionSettings--) | Istanzia le impostazioni per il metodo di compressione PPMd all'interno di un archivio 7z con ordine del modello predefinito e dimensione del sub-allocatore. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getMaxOrder()](#getMaxOrder--) | Restituisce l'ordine massimo. |
| [getMethod()](#getMethod--) | Ottiene il metodo di compressione o decompressione. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Restituisce la dimensione del sub-allocatore in MB. |
### SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize) {#SevenZipPPMdCompressionSettings-int-int-}
```
public SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)
```


Istanzia le impostazioni per il metodo di compressione PPMd all'interno di un archivio 7z.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32)))) {
archive.createEntry("data.bin", "data.bin");
archive.save("zipFile.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| maxOrder | int | Maximum order.

Bigger model orders almost surely results in better compression and surely more memory and CPU usage. |
| suballocatorSize | int | Memory size in MB suballocator may consume.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse. |

### SevenZipPPMdCompressionSettings() {#SevenZipPPMdCompressionSettings--}
```
public SevenZipPPMdCompressionSettings()
```


Instantiates settings for PPMd compression method within 7z archive with default model order and sub-allocator size.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("sevenZipFile.7z");
     }
 
```

L'ordine del modello predefinito è 6 e la dimensione del sub-allocatore è 16 MB.

### getMaxOrder() {#getMaxOrder--}
```
public final byte getMaxOrder()
```


Restituisce l'ordine massimo.

**Returns:**
byte - l'ordine massimo
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Ottiene il metodo di compressione o decompressione.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Restituisce la dimensione del sub-allocatore in MB.

**Returns:**
int - la dimensione del sub-allocatore in MB
