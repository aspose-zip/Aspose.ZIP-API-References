---
title: "Bzip2CompressionSettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen voor Bzip2-compressie binnen een ZIP-archief."
type: docs
weight: 41
url: /nl/java/com.aspose.zip/bzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class Bzip2CompressionSettings extends CompressionSettings
```

Instellingen voor Bzip2-compressie binnen een ZIP-archief.

bzip2 comprimeert bestanden met behulp van het Burrows-Wheeler bloksorteringstekstcompressie-algoritme en Huffman-codering.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Bzip2CompressionSettings(int blockSize)](#Bzip2CompressionSettings-int-) | Initialiseert een nieuw exemplaar van de [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) klasse. |
| [Bzip2CompressionSettings()](#Bzip2CompressionSettings--) | Initialiseert een nieuw exemplaar van de [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) klasse met de standaard blokgrootte, gelijk aan 9 honderd kilobytes. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Blokgrootte in honderden kilobytes. |
### Bzip2CompressionSettings(int blockSize) {#Bzip2CompressionSettings-int-}
```
public Bzip2CompressionSettings(int blockSize)
```


Initialiseert een nieuw exemplaar van de [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) klasse.

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


Blokgrootte in honderden kilobytes.

**Returns:**
int - blokgrootte in honderden kilobytes
