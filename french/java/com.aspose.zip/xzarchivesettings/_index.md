---
title: "XzArchiveSettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "La classe contient un ensemble de paramètres pour une archive xz particulière."
type: docs
weight: 147
url: /fr/java/com.aspose.zip/xzarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class XzArchiveSettings
```

La classe contient un ensemble de paramètres pour une archive xz particulière.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [XzArchiveSettings()](#XzArchiveSettings--) | Initialise une nouvelle instance de la classe [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) en utilisant une compression LZMA2 unique. |
| [XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)](#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-) | Initialise une nouvelle instance de la classe [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) avec des paramètres personnalisés. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Obtient le nombre de threads de compression. |
| [getFastSpeed()](#getFastSpeed--) | Obtient l'instance de la classe [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) avec une taille de dictionnaire égale à 1 mégaoctet dans le filtre LZMA2, une taille de bloc égale à 4 mégaoctets et une somme de contrôle CRC32. |
| [getFastestSpeed()](#getFastestSpeed--) | Obtient l'instance de la classe [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) avec une taille de dictionnaire égale à 65536 octets dans le filtre LZMA2, une taille de bloc égale à 1 mégaoctet et une somme de contrôle CRC32. |
| [getHighCompression()](#getHighCompression--) | Obtient l'instance de la classe [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) avec une taille de dictionnaire égale à 32 mégaoctets dans le filtre LZMA2, une taille de bloc égale à 128 mégaoctets et une somme de contrôle CRC32. |
| [getMaximumCompression()](#getMaximumCompression--) | Obtient l'instance de la classe [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) avec une taille de dictionnaire égale à 64 mégaoctets dans le filtre LZMA2, une taille de bloc égale à 256 mégaoctets et une somme de contrôle CRC32. |
| [getNormal()](#getNormal--) | Obtient l'instance de la classe [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) avec une taille de dictionnaire égale à 16 mégaoctets dans le filtre LZMA2, une taille de bloc égale à 64 mégaoctets et une somme de contrôle CRC32. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Définit le nombre de threads de compression. |
### XzArchiveSettings() {#XzArchiveSettings--}
```
public XzArchiveSettings()
```


Initialise une nouvelle instance de la classe [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) en utilisant une compression LZMA2 unique.

Le dictionnaire par défaut dans le filtre LZMA2 a une taille de 16 mégaoctets, la taille de bloc par défaut est de 64 mégaoctets, le type de somme de contrôle par défaut est CRC32.

### XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType) {#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-}
```
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```


Initialise une nouvelle instance de la classe [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) avec des paramètres personnalisés.

```

``````

try (FileOutputStream xzFile = new FileOutputStream(\"archive.xz\")) {
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

