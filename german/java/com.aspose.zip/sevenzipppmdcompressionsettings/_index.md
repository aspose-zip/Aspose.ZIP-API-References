---
title: "SevenZipPPMdCompressionSettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen für die PPMd-Kompressionsmethode innerhalb eines 7z-Archivs."
type: docs
weight: 117
url: /de/java/com.aspose.zip/sevenzipppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public final class SevenZipPPMdCompressionSettings extends SevenZipCompressionSettings
```

Einstellungen für die PPMd-Kompressionsmethode innerhalb eines 7z-Archivs.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)](#SevenZipPPMdCompressionSettings-int-int-) | Instanziiert Einstellungen für die PPMd-Komprimierungsmethode innerhalb eines 7z-Archivs. |
| [SevenZipPPMdCompressionSettings()](#SevenZipPPMdCompressionSettings--) | Instanziiert Einstellungen für die PPMd-Komprimierungsmethode innerhalb eines 7z-Archivs mit Standard‑Modellreihenfolge und Sub‑Allocator‑Größe. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getMaxOrder()](#getMaxOrder--) | Liefert die maximale Reihenfolge. |
| [getMethod()](#getMethod--) | Liefert die Komprimierungs- oder Dekomprimierungsmethode. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Liefert die Sub‑Allocator‑Größe in MB. |
### SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize) {#SevenZipPPMdCompressionSettings-int-int-}
```
public SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)
```


Instanziiert Einstellungen für die PPMd-Komprimierungsmethode innerhalb eines 7z-Archivs.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32)))) {
archive.createEntry("data.bin", "data.bin");
archive.save(\"zipFile.zip\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| maxOrder | int | Maximum order.

Bigger model orders almost surely results in better compression and surely more memory and CPU usage. |
| suballocatorSize | int | Memory size in MB suballocator may consume.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse. |

### SevenZipPPMdCompressionSettings() {#SevenZipPPMdCompressionSettings--}
```
public SevenZipPPMdCompressionSettings()
```


Instantiates settings for PPMd compression method within 7z archive with default model order and sub-allocator size.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("sevenZipFile.7z");
     }
 
```

Die Standard‑Modellreihenfolge ist 6 und die Sub‑Allocator‑Größe beträgt 16 MB.

### getMaxOrder() {#getMaxOrder--}
```
public final byte getMaxOrder()
```


Liefert die maximale Reihenfolge.

**Returns:**
byte – die maximale Reihenfolge
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Liefert die Komprimierungs- oder Dekomprimierungsmethode.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Liefert die Sub‑Allocator‑Größe in MB.

**Returns:**
int – die Sub‑Allocator‑Größe in MB
