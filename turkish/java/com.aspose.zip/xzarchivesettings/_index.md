---
title: "XzArchiveSettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Sınıf, belirli bir xz arşivi için bir dizi ayar içerir."
type: docs
weight: 147
url: /tr/java/com.aspose.zip/xzarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class XzArchiveSettings
```

Sınıf, belirli bir xz arşivi için bir dizi ayar içerir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [XzArchiveSettings()](#XzArchiveSettings--) | Tek LZMA2 sıkıştırması kullanarak yeni bir [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) sınıfının örneğini başlatır. |
| [XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)](#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-) | Özel parametrelerle yeni bir [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) sınıfının örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Sıkıştırma iş parçacığı sayısını alır. |
| [getFastSpeed()](#getFastSpeed--) | LZMA2 filtresinde sözlük boyutu 1 megabayt, blok boyutu 4 megabayt ve CRC32 sağlama değeri olan [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) sınıfının örneğini alır. |
| [getFastestSpeed()](#getFastestSpeed--) | LZMA2 filtresinde sözlük boyutu 65536 bayt, blok boyutu 1 megabayt ve CRC32 sağlama değeri olan [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) sınıfının örneğini alır. |
| [getHighCompression()](#getHighCompression--) | LZMA2 filtresinde sözlük boyutu 32 megabayt, blok boyutu 128 megabayt ve CRC32 sağlama değeri olan [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) sınıfının örneğini alır. |
| [getMaximumCompression()](#getMaximumCompression--) | LZMA2 filtresinde sözlük boyutu 64 megabayt, blok boyutu 256 megabayt ve CRC32 sağlama değeri olan [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) sınıfının örneğini alır. |
| [getNormal()](#getNormal--) | LZMA2 filtresinde sözlük boyutu 16 megabayt, blok boyutu 64 megabayt ve CRC32 sağlama değeri olan [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) sınıfının örneğini alır. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Sıkıştırma iş parçacığı sayısını ayarlar. |
### XzArchiveSettings() {#XzArchiveSettings--}
```
public XzArchiveSettings()
```


Tek LZMA2 sıkıştırması kullanarak yeni bir [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) sınıfının örneğini başlatır.

LZMA2 filtresindeki varsayılan sözlük boyutu 16 megabayt, varsayılan blok boyutu 64 megabayt ve varsayılan sağlama türü CRC32'tür.

### XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType) {#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-}
```
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```


Özel parametrelerle yeni bir [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) sınıfının örneğini başlatır.

```

``````

try (FileOutputStream xzFile = new FileOutputStream("archive.xz")) {
XzLZMA2FilterSettings filter = new XzLZMA2FilterSettings(5242880);
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {filter}, 10485760, XzCheckType.Crc32);
try (XzArchive archive = new XzArchive(settings)) {
archive.setSource(\"data.bin\");
archive.save(xzFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filters | [XzFilterSettings\[\]](../../com.aspose.zip/xzfiltersettings) | filters (compressors) to be sequentially applied to create [XzArchive](../../com.aspose.zip/xzarchive). It can be either single [XzLZMA2FilterSettings](../../com.aspose.zip/xzlzma2filtersettings) or pair of [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings) and [XzLZMA2FilterSettings](../../com.aspose.zip/xzlzma2filtersettings) |
| blockSize | long | size xz archive block |
| checkType | [XzCheckType](../../com.aspose.zip/xzchecktype) | type of checksum calculation for uncompressed data |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Gets compression thread count. If the value is greater than 1, multithreading compression will be used.

**Returns:**
int - compression thread count.
### getFastSpeed() {#getFastSpeed--}
```
public static XzArchiveSettings getFastSpeed()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 1 megabyte in LZMA2 filter, block size equals to 4 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the fast speed
### getFastestSpeed() {#getFastestSpeed--}
```
public static XzArchiveSettings getFastestSpeed()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 65536 bytes in LZMA2 filter, block size equals to 1 megabyte and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the fastest speed
### getHighCompression() {#getHighCompression--}
```
public static XzArchiveSettings getHighCompression()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 32 megabytes in LZMA2 filter, block size equals to 128 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the high compression
### getMaximumCompression() {#getMaximumCompression--}
```
public static XzArchiveSettings getMaximumCompression()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 64 megabytes in LZMA2 filter, block size equals to 256 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the maximum compression
### getNormal() {#getNormal--}
```
public static XzArchiveSettings getNormal()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 16 megabytes in LZMA2 filter, block size equals to 64 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with normal parameters
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Sets compression thread count. If the value is greater than 1, multithreading compression will be used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | compression thread count.

Do not set this number more than CPU cores |

