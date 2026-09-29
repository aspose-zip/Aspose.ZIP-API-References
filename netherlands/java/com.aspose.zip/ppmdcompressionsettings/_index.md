---
title: "PPMdCompressionSettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen voor PPMd-compressie binnen een ZIP-archief."
type: docs
weight: 93
url: /nl/java/com.aspose.zip/ppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class PPMdCompressionSettings extends CompressionSettings
```

Instellingen voor PPMd-compressie binnen een ZIP-archief.

PPMd is een data-compressie-algoritme ontwikkeld door Dmitry Shkarin. Dit algoritme is gebaseerd op voorspellende frase‑matching in meerdere order‑contexten.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [PPMdCompressionSettings(int modelOrder, int suballocatorSize)](#PPMdCompressionSettings-int-int-) | Initialiseert een nieuw exemplaar van de [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) klasse. |
| [PPMdCompressionSettings()](#PPMdCompressionSettings--) | Initialiseert een nieuw exemplaar van de [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) klasse met standaard modelorder en sub‑allocator‑grootte. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getModelOrder()](#getModelOrder--) | Haalt de order van het model op. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Haalt de sub-allocator-grootte op in MB. |
### PPMdCompressionSettings(int modelOrder, int suballocatorSize) {#PPMdCompressionSettings-int-int-}
```
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```


Initialiseert een nieuw exemplaar van de [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) klasse.

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

De standaard modelorder is 8, en de sub‑allocator‑grootte is 50 MB.

### getModelOrder() {#getModelOrder--}
```
public final int getModelOrder()
```


Haalt de order van het model op.

**Returns:**
int - de order van het model
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Haalt de sub-allocator-grootte op in MB.

**Returns:**
int - de sub-allocator-grootte in MB
