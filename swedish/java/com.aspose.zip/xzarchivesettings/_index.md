---
title: "XzArchiveSettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Klassen innehåller en uppsättning inställningar för ett specifikt xz-arkiv."
type: docs
weight: 147
url: /sv/java/com.aspose.zip/xzarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class XzArchiveSettings
```

Klassen innehåller en uppsättning inställningar för ett specifikt xz-arkiv.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [XzArchiveSettings()](#XzArchiveSettings--) | Initierar en ny instans av klassen [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) med enkel LZMA2-komprimering. |
| [XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)](#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-) | Initierar en ny instans av klassen [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) med anpassade parametrar. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Hämtar antalet komprimeringstrådar. |
| [getFastSpeed()](#getFastSpeed--) | Hämtar instansen av klassen [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) med en ordboksstorlek på 1 megabyte i LZMA2-filter, blockstorlek på 4 megabyte och CRC32-kontrollsumma. |
| [getFastestSpeed()](#getFastestSpeed--) | Hämtar instansen av klassen [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) med en ordboksstorlek på 65536 byte i LZMA2-filter, blockstorlek på 1 megabyte och CRC32-kontrollsumma. |
| [getHighCompression()](#getHighCompression--) | Hämtar instansen av klassen [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) med en ordboksstorlek på 32 megabyte i LZMA2-filter, blockstorlek på 128 megabyte och CRC32-kontrollsumma. |
| [getMaximumCompression()](#getMaximumCompression--) | Hämtar instansen av klassen [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) med en ordboksstorlek på 64 megabyte i LZMA2-filter, blockstorlek på 256 megabyte och CRC32-kontrollsumma. |
| [getNormal()](#getNormal--) | Hämtar instansen av klassen [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) med en ordboksstorlek på 16 megabyte i LZMA2-filter, blockstorlek på 64 megabyte och CRC32-kontrollsumma. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Ställer in antalet komprimeringstrådar. |
### XzArchiveSettings() {#XzArchiveSettings--}
```
public XzArchiveSettings()
```


Initierar en ny instans av klassen [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) med enkel LZMA2-komprimering.

Standardordbok i LZMA2-filter har en storlek på 16 megabyte, standardblockstorlek är 64 megabyte, och standardtyp för kontrollsumma är CRC32.

### XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType) {#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-}
```
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```


Initierar en ny instans av klassen [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) med anpassade parametrar.

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

