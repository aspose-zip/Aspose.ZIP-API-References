---
title: "Bzip2CompressionSettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Inställningar för Bzip2-komprimering i ett ZIP-arkiv."
type: docs
weight: 41
url: /sv/java/com.aspose.zip/bzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class Bzip2CompressionSettings extends CompressionSettings
```

Inställningar för Bzip2-komprimering i ett ZIP-arkiv.

bzip2 komprimerar filer med hjälp av Burrows‑Wheeler blocksorterings‑textkomprimeringsalgoritmen och Huffman‑kodning.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Bzip2CompressionSettings(int blockSize)](#Bzip2CompressionSettings-int-) | Initierar en ny instans av klassen [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings). |
| [Bzip2CompressionSettings()](#Bzip2CompressionSettings--) | Initierar en ny instans av klassen [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) med standardblockstorlek, motsvarande 9 hundra kilobyte. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Blockstorlek i hundra kilobyte. |
### Bzip2CompressionSettings(int blockSize) {#Bzip2CompressionSettings-int-}
```
public Bzip2CompressionSettings(int blockSize)
```


Initierar en ny instans av klassen [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings).

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


Blockstorlek i hundra kilobyte.

**Returns:**
int - blockstorlek i hundra kilobyte
