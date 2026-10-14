---
title: "XarBzip2CompressionSettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bzip2 sıkıştırma yöntemi için ayarlar."
type: docs
weight: 137
url: /tr/java/com.aspose.zip/xarbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings)
```
public class XarBzip2CompressionSettings extends XarCompressionSettings
```

Bzip2 sıkıştırma yöntemi için ayarlar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [XarBzip2CompressionSettings(int blockSize)](#XarBzip2CompressionSettings-int-) | Yeni bir [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) sınıfı örneği başlatır. |
| [XarBzip2CompressionSettings()](#XarBzip2CompressionSettings--) | Varsayılan blok boyutu 9 yüz kilobayt olan yeni bir [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Blok boyutu yüz kilobyte cinsinden. |
### XarBzip2CompressionSettings(int blockSize) {#XarBzip2CompressionSettings-int-}
```
public XarBzip2CompressionSettings(int blockSize)
```


Yeni bir [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) sınıfı örneği başlatır.

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
