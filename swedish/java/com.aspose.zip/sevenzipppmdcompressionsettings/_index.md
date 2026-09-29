---
title: "SevenZipPPMdCompressionSettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Inställningar för PPMd-komprimeringsmetod i ett 7z-arkiv."
type: docs
weight: 117
url: /sv/java/com.aspose.zip/sevenzipppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public final class SevenZipPPMdCompressionSettings extends SevenZipCompressionSettings
```

Inställningar för PPMd-komprimeringsmetod i ett 7z-arkiv.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)](#SevenZipPPMdCompressionSettings-int-int-) | Instansierar inställningar för PPMd-komprimeringsmetoden i ett 7z-arkiv. |
| [SevenZipPPMdCompressionSettings()](#SevenZipPPMdCompressionSettings--) | Instansierar inställningar för PPMd-komprimeringsmetoden i ett 7z-arkiv med standard modellordning och suballokeringsstorlek. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getMaxOrder()](#getMaxOrder--) | Hämtar den maximala ordningen. |
| [getMethod()](#getMethod--) | Hämtar komprimerings- eller dekomprimeringsmetod. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Hämtar suballokeringsstorleken i MB. |
### SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize) {#SevenZipPPMdCompressionSettings-int-int-}
```
public SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)
```


Instansierar inställningar för PPMd-komprimeringsmetoden i ett 7z-arkiv.

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

Standardmodellordningen är 6 och suballokeringsstorleken är 16MB.

### getMaxOrder() {#getMaxOrder--}
```
public final byte getMaxOrder()
```


Hämtar den maximala ordningen.

**Returns:**
byte - den maximala ordningen
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Hämtar komprimerings- eller dekomprimeringsmetod.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Hämtar suballokeringsstorleken i MB.

**Returns:**
int - suballokeringsstorleken i MB
