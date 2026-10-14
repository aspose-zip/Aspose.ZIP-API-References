---
title: "XzArchiveSettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "الفئة تحتوي على مجموعة من الإعدادات لأرشيف xz معين."
type: docs
weight: 147
url: /ar/java/com.aspose.zip/xzarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class XzArchiveSettings
```

الفئة تحتوي على مجموعة من الإعدادات لأرشيف xz معين.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [XzArchiveSettings()](#XzArchiveSettings--) | يُنشئ مثلاً جديداً من الفئة [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) باستخدام ضغط LZMA2 واحد. |
| [XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)](#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-) | يُنشئ مثلاً جديداً من الفئة [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) بمعلمات مخصصة. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | يحصل على عدد خيوط الضغط. |
| [getFastSpeed()](#getFastSpeed--) | يحصل على نسخة من الفئة [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) بحجم القاموس يساوي 1 ميغابايت في مرشح LZMA2، وحجم الكتلة يساوي 4 ميغابايت وتحقق CRC32. |
| [getFastestSpeed()](#getFastestSpeed--) | يحصل على نسخة من الفئة [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) بحجم القاموس يساوي 65536 بايت في مرشح LZMA2، وحجم الكتلة يساوي 1 ميغابايت وتحقق CRC32. |
| [getHighCompression()](#getHighCompression--) | يحصل على نسخة من الفئة [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) بحجم القاموس يساوي 32 ميغابايت في مرشح LZMA2، وحجم الكتلة يساوي 128 ميغابايت وتحقق CRC32. |
| [getMaximumCompression()](#getMaximumCompression--) | يحصل على نسخة من الفئة [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) بحجم القاموس يساوي 64 ميغابايت في مرشح LZMA2، وحجم الكتلة يساوي 256 ميغابايت وتحقق CRC32. |
| [getNormal()](#getNormal--) | يحصل على نسخة من الفئة [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) بحجم القاموس يساوي 16 ميغابايت في مرشح LZMA2، وحجم الكتلة يساوي 64 ميغابايت وتحقق CRC32. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | يضبط عدد خيوط الضغط. |
### XzArchiveSettings() {#XzArchiveSettings--}
```
public XzArchiveSettings()
```


يُنشئ مثلاً جديداً من الفئة [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) باستخدام ضغط LZMA2 واحد.

القاموس الافتراضي في مرشح LZMA2 حجمه يساوي 16 ميغابايت، حجم الكتلة الافتراضي يساوي 64 ميغابايت، نوع التحقق الافتراضي هو CRC32.

### XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType) {#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-}
```
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```


يُنشئ مثلاً جديداً من الفئة [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) بمعلمات مخصصة.

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

