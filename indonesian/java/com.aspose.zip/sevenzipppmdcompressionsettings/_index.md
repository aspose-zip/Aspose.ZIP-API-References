---
title: "SevenZipPPMdCompressionSettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan untuk metode kompresi PPMd dalam arsip 7z."
type: docs
weight: 117
url: /id/java/com.aspose.zip/sevenzipppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public final class SevenZipPPMdCompressionSettings extends SevenZipCompressionSettings
```

Pengaturan untuk metode kompresi PPMd dalam arsip 7z.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)](#SevenZipPPMdCompressionSettings-int-int-) | Membuat instance pengaturan untuk metode kompresi PPMd dalam arsip 7z. |
| [SevenZipPPMdCompressionSettings()](#SevenZipPPMdCompressionSettings--) | Membuat instance pengaturan untuk metode kompresi PPMd dalam arsip 7z dengan urutan model default dan ukuran sub-allocator. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getMaxOrder()](#getMaxOrder--) | Mendapatkan urutan maksimum. |
| [getMethod()](#getMethod--) | Mendapatkan metode kompresi atau dekompresi. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Mendapatkan ukuran sub-allocator dalam MB. |
### SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize) {#SevenZipPPMdCompressionSettings-int-int-}
```
public SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)
```


Membuat instance pengaturan untuk metode kompresi PPMd dalam arsip 7z.

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

Urutan model default adalah 6 dan ukuran sub-allocator adalah 16MB.

### getMaxOrder() {#getMaxOrder--}
```
public final byte getMaxOrder()
```


Mendapatkan urutan maksimum.

**Returns:**
byte - urutan maksimum
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Mendapatkan metode kompresi atau dekompresi.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Mendapatkan ukuran sub-allocator dalam MB.

**Returns:**
int - ukuran sub-allocator dalam MB
