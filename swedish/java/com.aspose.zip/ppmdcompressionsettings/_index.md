---
title: "PPMdCompressionSettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Inställningar för PPMd-komprimering i ett ZIP-arkiv."
type: docs
weight: 93
url: /sv/java/com.aspose.zip/ppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class PPMdCompressionSettings extends CompressionSettings
```

Inställningar för PPMd-komprimering i ett ZIP-arkiv.

PPMd är en datakomprimeringsalgoritm utvecklad av Dmitry Shkarin. Denna algoritm är baserad på prediktiv frasmatchning i flera ordningskontexter.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [PPMdCompressionSettings(int modelOrder, int suballocatorSize)](#PPMdCompressionSettings-int-int-) | Initierar en ny instans av klassen [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings). |
| [PPMdCompressionSettings()](#PPMdCompressionSettings--) | Initierar en ny instans av klassen [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) med standard modellordning och suballokeringsstorlek. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getModelOrder()](#getModelOrder--) | Hämtar modellens ordning. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Hämtar suballokeringsstorleken i MB. |
### PPMdCompressionSettings(int modelOrder, int suballocatorSize) {#PPMdCompressionSettings-int-int-}
```
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```


Initierar en ny instans av klassen [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10)))) {
archive.createEntry("data.bin", "data.bin");
archive.save("zipFile.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| modelOrder | int | Order of the model.

Bigger model orders almost surely results in better compression and surely more memory and CPU usage. |
| suballocatorSize | int | Memory size in MB suballocator may consume.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse. |

### PPMdCompressionSettings() {#PPMdCompressionSettings--}
```
public PPMdCompressionSettings()
```


Initializes a new instance of the [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) class with default model order and sub-allocator size.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("zipFile.zip");
     }
 
```

Standardmodellordningen är 8 och suballokeringsstorleken är 50 MB.

### getModelOrder() {#getModelOrder--}
```
public final int getModelOrder()
```


Hämtar modellens ordning.

**Returns:**
int - modellens ordning
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Hämtar suballokeringsstorleken i MB.

**Returns:**
int - suballokeringsstorleken i MB
