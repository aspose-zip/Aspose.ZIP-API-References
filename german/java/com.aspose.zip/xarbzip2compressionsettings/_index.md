---
title: "XarBzip2CompressionSettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen für die Bzip2-Komprimierungsmethode."
type: docs
weight: 137
url: /de/java/com.aspose.zip/xarbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings)
```
public class XarBzip2CompressionSettings extends XarCompressionSettings
```

Einstellungen für die Bzip2-Komprimierungsmethode.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [XarBzip2CompressionSettings(int blockSize)](#XarBzip2CompressionSettings-int-) | Initialisiert eine neue Instanz der [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings)-Klasse. |
| [XarBzip2CompressionSettings()](#XarBzip2CompressionSettings--) | Initialisiert eine neue Instanz der [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings)-Klasse mit der Standard-Blockgröße von 9 Hundert Kilobyte. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Blockgröße in Hunderten von Kilobyte. |
### XarBzip2CompressionSettings(int blockSize) {#XarBzip2CompressionSettings-int-}
```
public XarBzip2CompressionSettings(int blockSize)
```


Initialisiert eine neue Instanz der [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings)-Klasse.

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
