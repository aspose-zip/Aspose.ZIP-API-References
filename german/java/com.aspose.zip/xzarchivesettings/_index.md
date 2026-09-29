---
title: "XzArchiveSettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Die Klasse enthält eine Reihe von Einstellungen für ein bestimmtes xz-Archiv."
type: docs
weight: 147
url: /de/java/com.aspose.zip/xzarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class XzArchiveSettings
```

Die Klasse enthält eine Reihe von Einstellungen für ein bestimmtes xz-Archiv.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [XzArchiveSettings()](#XzArchiveSettings--) | Initialisiert eine neue Instanz der Klasse [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) mit einer einzelnen LZMA2-Kompression. |
| [XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)](#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-) | Initialisiert eine neue Instanz der Klasse [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) mit benutzerdefinierten Parametern. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Liefert die Anzahl der Komprimierungs-Threads. |
| [getFastSpeed()](#getFastSpeed--) | Ermittelt die Instanz der Klasse [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) mit einer Wörterbuchgröße von 1 Megabyte im LZMA2‑Filter, einer Blockgröße von 4 Megabyte und einer CRC32‑Prüfsumme. |
| [getFastestSpeed()](#getFastestSpeed--) | Ermittelt die Instanz der Klasse [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) mit einer Wörterbuchgröße von 65536 Bytes im LZMA2‑Filter, einer Blockgröße von 1 Megabyte und einer CRC32‑Prüfsumme. |
| [getHighCompression()](#getHighCompression--) | Ermittelt die Instanz der Klasse [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) mit einer Wörterbuchgröße von 32 Megabyte im LZMA2‑Filter, einer Blockgröße von 128 Megabyte und einer CRC32‑Prüfsumme. |
| [getMaximumCompression()](#getMaximumCompression--) | Ermittelt die Instanz der Klasse [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) mit einer Wörterbuchgröße von 64 Megabyte im LZMA2‑Filter, einer Blockgröße von 256 Megabyte und einer CRC32‑Prüfsumme. |
| [getNormal()](#getNormal--) | Ermittelt die Instanz der Klasse [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) mit einer Wörterbuchgröße von 16 Megabyte im LZMA2‑Filter, einer Blockgröße von 64 Megabyte und einer CRC32‑Prüfsumme. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Setzt die Anzahl der Komprimierungs-Threads. |
### XzArchiveSettings() {#XzArchiveSettings--}
```
public XzArchiveSettings()
```


Initialisiert eine neue Instanz der Klasse [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) mit einer einzelnen LZMA2-Kompression.

Standardwörterbuch im LZMA2-Filter hat eine Größe von 16 Megabyte, Standardblockgröße von 64 Megabyte, Standardprüfsummentyp ist CRC32.

### XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType) {#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-}
```
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```


Initialisiert eine neue Instanz der Klasse [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) mit benutzerdefinierten Parametern.

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

