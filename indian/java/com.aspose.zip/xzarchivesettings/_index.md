---
title: "XzArchiveSettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह क्लास विशेष xz अभिलेख के सेटिंग्स का संग्रह रखती है।"
type: docs
weight: 147
url: /hi/java/com.aspose.zip/xzarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class XzArchiveSettings
```

यह क्लास विशेष xz अभिलेख के सेटिंग्स का संग्रह रखती है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [XzArchiveSettings()](#XzArchiveSettings--) | एक नया उदाहरण प्रारंभ करता है [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) क्लास का, एकल LZMA2 संपीड़न का उपयोग करके। |
| [XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)](#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-) | कस्टम पैरामीटरों के साथ [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) क्लास का नया उदाहरण प्रारंभ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | कम्प्रेशन थ्रेड की संख्या प्राप्त करता है। |
| [getFastSpeed()](#getFastSpeed--) | LZMA2 फ़िल्टर में शब्दकोश आकार 1 मेगाबाइट, ब्लॉक आकार 4 मेगाबाइट और CRC32 चेकसम के साथ [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) क्लास का इंस्टेंस प्राप्त करता है। |
| [getFastestSpeed()](#getFastestSpeed--) | LZMA2 फ़िल्टर में शब्दकोश आकार 65536 बाइट, ब्लॉक आकार 1 मेगाबाइट और CRC32 चेकसम के साथ [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) क्लास का इंस्टेंस प्राप्त करता है। |
| [getHighCompression()](#getHighCompression--) | LZMA2 फ़िल्टर में शब्दकोश आकार 32 मेगाबाइट, ब्लॉक आकार 128 मेगाबाइट और CRC32 चेकसम के साथ [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) क्लास का इंस्टेंस प्राप्त करता है। |
| [getMaximumCompression()](#getMaximumCompression--) | LZMA2 फ़िल्टर में शब्दकोश आकार 64 मेगाबाइट, ब्लॉक आकार 256 मेगाबाइट और CRC32 चेकसम के साथ [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) क्लास का इंस्टेंस प्राप्त करता है। |
| [getNormal()](#getNormal--) | LZMA2 फ़िल्टर में शब्दकोश आकार 16 मेगाबाइट, ब्लॉक आकार 64 मेगाबाइट और CRC32 चेकसम के साथ [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) क्लास का इंस्टेंस प्राप्त करता है। |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | कम्प्रेशन थ्रेड की संख्या सेट करता है। |
### XzArchiveSettings() {#XzArchiveSettings--}
```
public XzArchiveSettings()
```


एक नया उदाहरण प्रारंभ करता है [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) क्लास का, एकल LZMA2 संपीड़न का उपयोग करके।

डिफ़ॉल्ट शब्दकोश LZMA2 फ़िल्टर में 16 मेगाबाइट, डिफ़ॉल्ट ब्लॉक आकार 64 मेगाबाइट, डिफ़ॉल्ट चेकसम प्रकार CRC32 है।

### XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType) {#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-}
```
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```


कस्टम पैरामीटरों के साथ [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) क्लास का नया उदाहरण प्रारंभ करता है।

```

``````

try (FileOutputStream xzFile = new FileOutputStream(\"archive.xz\")) {
XzLZMA2FilterSettings filter = new XzLZMA2FilterSettings(5242880);
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {filter}, 10485760, XzCheckType.Crc32);
try (XzArchive archive = new XzArchive(settings)) {
archive.setSource("data.bin");
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

