---
title: "XarBzip2CompressionSettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres pour la méthode de compression Bzip2."
type: docs
weight: 137
url: /fr/java/com.aspose.zip/xarbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings)
```
public class XarBzip2CompressionSettings extends XarCompressionSettings
```

Paramètres pour la méthode de compression Bzip2.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [XarBzip2CompressionSettings(int blockSize)](#XarBzip2CompressionSettings-int-) | Initialise une nouvelle instance de la classe [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings). |
| [XarBzip2CompressionSettings()](#XarBzip2CompressionSettings--) | Initialise une nouvelle instance de la classe [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) avec une taille de bloc par défaut, égale à 9 centaines de kilooctets. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Taille du bloc en centaines de kilo-octets. |
### XarBzip2CompressionSettings(int blockSize) {#XarBzip2CompressionSettings-int-}
```
public XarBzip2CompressionSettings(int blockSize)
```


Initialise une nouvelle instance de la classe [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings).

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
