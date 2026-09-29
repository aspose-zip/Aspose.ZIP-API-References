---
title: "SevenZipPPMdCompressionSettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen voor PPMd-compressiemethode binnen een 7z-archief."
type: docs
weight: 117
url: /nl/java/com.aspose.zip/sevenzipppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public final class SevenZipPPMdCompressionSettings extends SevenZipCompressionSettings
```

Instellingen voor PPMd-compressiemethode binnen een 7z-archief.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)](#SevenZipPPMdCompressionSettings-int-int-) | Instantieert instellingen voor de PPMd-compressiemethode binnen een 7z-archief. |
| [SevenZipPPMdCompressionSettings()](#SevenZipPPMdCompressionSettings--) | Instantieert instellingen voor de PPMd-compressiemethode binnen een 7z-archief met de standaard modelvolgorde en sub-allocator-grootte. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getMaxOrder()](#getMaxOrder--) | Haalt de maximale volgorde op. |
| [getMethod()](#getMethod--) | Haalt compressie- of decompressiemethode op. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Haalt de sub-allocator-grootte op in MB. |
### SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize) {#SevenZipPPMdCompressionSettings-int-int-}
```
public SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)
```


Instantieert instellingen voor de PPMd-compressiemethode binnen een 7z-archief.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32)))) {
archive.createEntry("data.bin", "data.bin");
archive.save("zipFile.zip");
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

De standaard modelvolgorde is 6 en de sub-allocator-grootte is 16 MB.

### getMaxOrder() {#getMaxOrder--}
```
public final byte getMaxOrder()
```


Haalt de maximale volgorde op.

**Returns:**
byte - de maximale volgorde
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Haalt compressie- of decompressiemethode op.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Haalt de sub-allocator-grootte op in MB.

**Returns:**
int - de sub-allocator-grootte in MB
