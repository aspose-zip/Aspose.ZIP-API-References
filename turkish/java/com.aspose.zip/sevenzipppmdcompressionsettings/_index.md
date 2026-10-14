---
title: "SevenZipPPMdCompressionSettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "7z arşivi içinde PPMd sıkıştırma yöntemi için ayarlar."
type: docs
weight: 117
url: /tr/java/com.aspose.zip/sevenzipppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public final class SevenZipPPMdCompressionSettings extends SevenZipCompressionSettings
```

7z arşivi içinde PPMd sıkıştırma yöntemi için ayarlar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)](#SevenZipPPMdCompressionSettings-int-int-) | 7z arşivindeki PPMd sıkıştırma yöntemi için ayarları örnekler. |
| [SevenZipPPMdCompressionSettings()](#SevenZipPPMdCompressionSettings--) | 7z arşivindeki PPMd sıkıştırma yöntemi için varsayılan model sırası ve alt-ayırıcı boyutu ile ayarları örnekler. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getMaxOrder()](#getMaxOrder--) | Maksimum sırayı alır. |
| [getMethod()](#getMethod--) | Sıkıştırma veya açma yöntemini alır. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Alt-ayırıcı boyutunu MB cinsinden alır. |
### SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize) {#SevenZipPPMdCompressionSettings-int-int-}
```
public SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)
```


7z arşivindeki PPMd sıkıştırma yöntemi için ayarları örnekler.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32)))) {
archive.createEntry(\"data.bin\", \"data.bin\");
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

Varsayılan model sırası 6 ve alt-ayırıcı boyutu 16MB'dir.

### getMaxOrder() {#getMaxOrder--}
```
public final byte getMaxOrder()
```


Maksimum sırayı alır.

**Returns:**
byte - maksimum sıra
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Sıkıştırma veya açma yöntemini alır.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Alt-ayırıcı boyutunu MB cinsinden alır.

**Returns:**
int - alt-ayırıcı boyutu MB cinsinden
