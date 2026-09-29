---
title: "XarBzip2CompressionSettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan untuk metode kompresi Bzip2."
type: docs
weight: 137
url: /id/java/com.aspose.zip/xarbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings)
```
public class XarBzip2CompressionSettings extends XarCompressionSettings
```

Pengaturan untuk metode kompresi Bzip2.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [XarBzip2CompressionSettings(int blockSize)](#XarBzip2CompressionSettings-int-) | Menginisialisasi instance baru dari kelas [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings). |
| [XarBzip2CompressionSettings()](#XarBzip2CompressionSettings--) | Menginisialisasi instance baru dari kelas [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) dengan ukuran blok default, setara dengan 9 ratus kilobyte. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Ukuran blok dalam ratus kilobyte. |
### XarBzip2CompressionSettings(int blockSize) {#XarBzip2CompressionSettings-int-}
```
public XarBzip2CompressionSettings(int blockSize)
```


Menginisialisasi instance baru dari kelas [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings).

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
