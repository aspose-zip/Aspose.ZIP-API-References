---
title: "Bzip2CompressionSettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "ZIP arşivi içinde Bzip2 sıkıştırması için ayarlar."
type: docs
weight: 41
url: /tr/java/com.aspose.zip/bzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class Bzip2CompressionSettings extends CompressionSettings
```

ZIP arşivi içinde Bzip2 sıkıştırması için ayarlar.

bzip2, dosyaları Burrows-Wheeler blok sıralama metin sıkıştırma algoritması ve Huffman kodlaması kullanarak sıkıştırır.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Bzip2CompressionSettings(int blockSize)](#Bzip2CompressionSettings-int-) | Yeni bir [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) sınıfı örneği başlatır. |
| [Bzip2CompressionSettings()](#Bzip2CompressionSettings--) | Varsayılan blok boyutu 900 kilobyte olan yeni bir [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Blok boyutu yüz kilobyte cinsinden. |
### Bzip2CompressionSettings(int blockSize) {#Bzip2CompressionSettings-int-}
```
public Bzip2CompressionSettings(int blockSize)
```


Yeni bir [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) sınıfı örneği başlatır.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1)))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(zipFile);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | Block size in hundreds of kilobytes. |

### Bzip2CompressionSettings() {#Bzip2CompressionSettings--}
```
public Bzip2CompressionSettings()
```


Initializes a new instance of the [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) class with default block size, equals to 9 hundred of kilobytes.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save(zipFile);
     }
 
```



### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Blok boyutu yüz kilobyte cinsinden.

**Returns:**
int - blok boyutu yüz kilobyte cinsinden
