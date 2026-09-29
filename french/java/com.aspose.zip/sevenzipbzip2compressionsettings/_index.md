---
title: "SevenZipBZip2CompressionSettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres pour la méthode de compression BZip2 dans une archive 7z."
type: docs
weight: 109
url: /fr/java/com.aspose.zip/sevenzipbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipBZip2CompressionSettings extends SevenZipCompressionSettings
```

Paramètres pour la méthode de compression BZip2 dans une archive 7z.

Bzip2 compresse les fichiers en utilisant l'algorithme de compression de texte par tri de blocs Burrows‑Wheeler et le codage Huffman.

Voir plus : [Bzip2][]


[Bzip2]: https://en.wikipedia.org/wiki/Bzip2
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SevenZipBZip2CompressionSettings(int blockSize)](#SevenZipBZip2CompressionSettings-int-) | Initialise une nouvelle instance de la classe [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings). |
| [SevenZipBZip2CompressionSettings()](#SevenZipBZip2CompressionSettings--) | Initialise une nouvelle instance de la classe [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) avec la taille de bloc par défaut, égale à 9 centaines de kilo-octets. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Taille du bloc en centaines de kilo-octets. |
| [getMethod()](#getMethod--) | Obtient la méthode de compression ou de décompression. |
### SevenZipBZip2CompressionSettings(int blockSize) {#SevenZipBZip2CompressionSettings-int-}
```
public SevenZipBZip2CompressionSettings(int blockSize)
```


Initialise une nouvelle instance de la classe [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| blockSize | int | taille du bloc en centaines de kilo-octets |

### SevenZipBZip2CompressionSettings() {#SevenZipBZip2CompressionSettings--}
```
public SevenZipBZip2CompressionSettings()
```


Initialise une nouvelle instance de la classe [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) avec la taille de bloc par défaut, égale à 9 centaines de kilo-octets.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Taille du bloc en centaines de kilo-octets.

**Returns:**
int - taille du bloc en centaines de kilo-octets
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Obtient la méthode de compression ou de décompression.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
