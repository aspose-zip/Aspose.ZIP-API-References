---
title: "XarBzip2CompressionSettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen voor Bzip2-compressiemethode."
type: docs
weight: 137
url: /nl/java/com.aspose.zip/xarbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings)
```
public class XarBzip2CompressionSettings extends XarCompressionSettings
```

Instellingen voor Bzip2-compressiemethode.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [XarBzip2CompressionSettings(int blockSize)](#XarBzip2CompressionSettings-int-) | Initialiseert een nieuw exemplaar van de [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) klasse. |
| [XarBzip2CompressionSettings()](#XarBzip2CompressionSettings--) | Initialiseert een nieuw exemplaar van de [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) klasse met de standaard blokgrootte, gelijk aan 9 honderd kilobytes. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Blokgrootte in honderden kilobytes. |
### XarBzip2CompressionSettings(int blockSize) {#XarBzip2CompressionSettings-int-}
```
public XarBzip2CompressionSettings(int blockSize)
```


Initialiseert een nieuw exemplaar van de [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) klasse.

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
