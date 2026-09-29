---
title: "PPMdCompressionSettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen für PPMd-Kompression innerhalb eines ZIP-Archivs."
type: docs
weight: 93
url: /de/java/com.aspose.zip/ppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class PPMdCompressionSettings extends CompressionSettings
```

Einstellungen für PPMd-Kompression innerhalb eines ZIP-Archivs.

PPMd ist ein Datenkompressionsalgorithmus, der von Dmitry Shkarin entwickelt wurde. Dieser Algorithmus basiert auf prädiktivem Phrasenabgleich in mehreren Ordnungs-Kontexten.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PPMdCompressionSettings(int modelOrder, int suballocatorSize)](#PPMdCompressionSettings-int-int-) | Initialisiert eine neue Instanz der Klasse [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings). |
| [PPMdCompressionSettings()](#PPMdCompressionSettings--) | Initialisiert eine neue Instanz der Klasse [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) mit Standard-Modellordnung und Sub-Allocator-Größe. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getModelOrder()](#getModelOrder--) | Liefert die Ordnung des Modells. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Liefert die Sub‑Allocator‑Größe in MB. |
### PPMdCompressionSettings(int modelOrder, int suballocatorSize) {#PPMdCompressionSettings-int-int-}
```
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```


Initialisiert eine neue Instanz der Klasse [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10)))) {
archive.createEntry("data.bin", "data.bin");
archive.save(\"zipFile.zip\");
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

Die Standard-Modellordnung ist 8 und die Sub-Allocator-Größe beträgt 50 MB.

### getModelOrder() {#getModelOrder--}
```
public final int getModelOrder()
```


Liefert die Ordnung des Modells.

**Returns:**
int – die Ordnung des Modells
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Liefert die Sub‑Allocator‑Größe in MB.

**Returns:**
int – die Sub‑Allocator‑Größe in MB
