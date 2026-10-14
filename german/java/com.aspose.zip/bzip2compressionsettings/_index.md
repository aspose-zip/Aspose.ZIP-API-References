---
title: "Bzip2CompressionSettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen für Bzip2-Kompression innerhalb eines ZIP-Archivs."
type: docs
weight: 41
url: /de/java/com.aspose.zip/bzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class Bzip2CompressionSettings extends CompressionSettings
```

Einstellungen für Bzip2-Kompression innerhalb eines ZIP-Archivs.

bzip2 komprimiert Dateien mit dem Burrows-Wheeler-Blocksortier-Textkompressionsalgorithmus und Huffman-Codierung.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Bzip2CompressionSettings(int blockSize)](#Bzip2CompressionSettings-int-) | Initialisiert eine neue Instanz der Klasse [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings). |
| [Bzip2CompressionSettings()](#Bzip2CompressionSettings--) | Initialisiert eine neue Instanz der Klasse [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) mit der Standardblockgröße, die 9 Hundert Kilobyte entspricht. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Blockgröße in Hunderten von Kilobyte. |
### Bzip2CompressionSettings(int blockSize) {#Bzip2CompressionSettings-int-}
```
public Bzip2CompressionSettings(int blockSize)
```


Initialisiert eine neue Instanz der Klasse [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings).

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


Blockgröße in Hunderten von Kilobyte.

**Returns:**
int - Blockgröße in Hunderten von Kilobyte
