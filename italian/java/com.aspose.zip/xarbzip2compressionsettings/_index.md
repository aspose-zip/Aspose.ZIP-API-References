---
title: "XarBzip2CompressionSettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni per il metodo di compressione Bzip2."
type: docs
weight: 137
url: /it/java/com.aspose.zip/xarbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings)
```
public class XarBzip2CompressionSettings extends XarCompressionSettings
```

Impostazioni per il metodo di compressione Bzip2.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [XarBzip2CompressionSettings(int blockSize)](#XarBzip2CompressionSettings-int-) | Inizializza una nuova istanza della classe [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings). |
| [XarBzip2CompressionSettings()](#XarBzip2CompressionSettings--) | Inizializza una nuova istanza della classe [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) con dimensione di blocco predefinita, pari a 9 centinaia di kilobyte. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Dimensione del blocco in centinaia di kilobyte. |
### XarBzip2CompressionSettings(int blockSize) {#XarBzip2CompressionSettings-int-}
```
public XarBzip2CompressionSettings(int blockSize)
```


Inizializza una nuova istanza della classe [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings).

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("data.bin", "data.bin", false, new XarBzip2CompressionSettings(1));
archive.save("archive.xar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | block size in hundreds of kilobytes |

### XarBzip2CompressionSettings() {#XarBzip2CompressionSettings--}
```
public XarBzip2CompressionSettings()
```


Initializes a new instance of the [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) class with default block size, equals to 9 hundred of kilobytes.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Block size in hundreds of kilobytes.

**Returns:**
int - block size in hundreds of kilobytes
