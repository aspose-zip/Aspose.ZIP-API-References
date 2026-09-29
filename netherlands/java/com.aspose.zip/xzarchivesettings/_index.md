---
title: "XzArchiveSettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "De klasse bevat een reeks instellingen voor een specifiek xz-archief."
type: docs
weight: 147
url: /nl/java/com.aspose.zip/xzarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class XzArchiveSettings
```

De klasse bevat een reeks instellingen voor een specifiek xz-archief.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [XzArchiveSettings()](#XzArchiveSettings--) | Initialiseert een nieuw exemplaar van de klasse [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) met enkele LZMA2-compressie. |
| [XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)](#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-) | Initialiseert een nieuw exemplaar van de klasse [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) met aangepaste parameters. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Haalt het aantal compressiedraden op. |
| [getFastSpeed()](#getFastSpeed--) | Haalt de instantie van de klasse [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) op met een woordenboekgrootte van 1 megabyte in de LZMA2-filter, een blokgrootte van 4 megabyte en een CRC32-controle. |
| [getFastestSpeed()](#getFastestSpeed--) | Haalt de instantie van de klasse [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) op met een woordenboekgrootte van 65536 bytes in de LZMA2-filter, een blokgrootte van 1 megabyte en een CRC32-controle. |
| [getHighCompression()](#getHighCompression--) | Haalt de instantie van de klasse [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) op met een woordenboekgrootte van 32 megabyte in de LZMA2-filter, een blokgrootte van 128 megabyte en een CRC32-controle. |
| [getMaximumCompression()](#getMaximumCompression--) | Haalt de instantie van de klasse [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) op met een woordenboekgrootte van 64 megabyte in de LZMA2-filter, een blokgrootte van 256 megabyte en een CRC32-controle. |
| [getNormal()](#getNormal--) | Haalt de instantie van de klasse [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) op met een woordenboekgrootte van 16 megabyte in de LZMA2-filter, een blokgrootte van 64 megabyte en een CRC32-controle. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Stelt het aantal compressiedraden in. |
### XzArchiveSettings() {#XzArchiveSettings--}
```
public XzArchiveSettings()
```


Initialiseert een nieuw exemplaar van de klasse [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) met enkele LZMA2-compressie.

Standaardwoordenboek in de LZMA2-filter heeft een grootte van 16 megabyte, standaard blokgrootte is 64 megabyte, een standaard controlesoort is CRC32.

### XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType) {#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-}
```
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```


Initialiseert een nieuw exemplaar van de klasse [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) met aangepaste parameters.

```

``````

try (FileOutputStream xzFile = new FileOutputStream("archive.xz")) {
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

