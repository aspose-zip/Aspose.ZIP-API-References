---
title: "Bzip2CompressionSettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres pour la compression Bzip2 dans une archive ZIP."
type: docs
weight: 41
url: /fr/java/com.aspose.zip/bzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class Bzip2CompressionSettings extends CompressionSettings
```

Paramètres pour la compression Bzip2 dans une archive ZIP.

bzip2 compresse les fichiers en utilisant l'algorithme de compression de texte par tri de blocs Burrows‑Wheeler et le codage Huffman.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Bzip2CompressionSettings(int blockSize)](#Bzip2CompressionSettings-int-) | Initialise une nouvelle instance de la classe [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings). |
| [Bzip2CompressionSettings()](#Bzip2CompressionSettings--) | Initialise une nouvelle instance de la classe [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) avec la taille de bloc par défaut, égale à 9 centaines de kilo-octets. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Taille du bloc en centaines de kilo-octets. |
### Bzip2CompressionSettings(int blockSize) {#Bzip2CompressionSettings-int-}
```
public Bzip2CompressionSettings(int blockSize)
```


Initialise une nouvelle instance de la classe [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1)))) {
archive.createEntry(\"data.bin\", \"data.bin\");
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


Taille du bloc en centaines de kilo-octets.

**Returns:**
int - taille du bloc en centaines de kilo-octets
