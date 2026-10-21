---
title: "LzipArchiveSettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Klassen innehåller inställningar för ett specifikt lzip-arkiv."
type: docs
weight: 84
url: /sv/java/com.aspose.zip/lziparchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzipArchiveSettings
```

Klassen innehåller inställningar för ett specifikt lzip-arkiv.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [LzipArchiveSettings(int dictionarySize)](#LzipArchiveSettings-int-) | Initierar en ny instans av [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) med en specifik ordboksstorlek. |
| [LzipArchiveSettings(int dictionarySize, int maxMemberSize)](#LzipArchiveSettings-int-int-) | Initierar en ny instans av [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) med en specifik ordboksstorlek. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Hämtar antalet komprimeringstrådar. |
| [getDictionarySize()](#getDictionarySize--) | Hämtar storleken på ordboken som används av LZMA-komprimering. |
| [getFastSpeed()](#getFastSpeed--) | Hämtar en instans av klassen [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) med ordboksstorlek lika med 1 megabyte i LZMA-filter. |
| [getFastestSpeed()](#getFastestSpeed--) | Hämtar en instans av klassen [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) med ordboksstorlek lika med 65536 byte i LZMA-filter. |
| [getHighCompression()](#getHighCompression--) | Hämtar en instans av klassen [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) med ordboksstorlek lika med 32 megabyte i LZMA-filter. |
| [getMaxMemberSize()](#getMaxMemberSize--) | Hämtar den maximala storleken för en medlem i lzip-arkivet, angiven i byte. |
| [getMaximumCompression()](#getMaximumCompression--) | Hämtar en instans av klassen [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) med ordboksstorlek lika med 64 megabyte i LZMA-filter. |
| [getNormal()](#getNormal--) | Hämtar en instans av klassen [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) med ordboksstorlek lika med 16 megabyte i LZMA-filter. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Ställer in antalet komprimeringstrådar. |
### LzipArchiveSettings(int dictionarySize) {#LzipArchiveSettings-int-}
```
public LzipArchiveSettings(int dictionarySize)
```


Initierar en ny instans av [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) med en specifik ordboksstorlek.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dictionarySize | int | ordboksstorlek för LZMA-komprimering i byte |

### LzipArchiveSettings(int dictionarySize, int maxMemberSize) {#LzipArchiveSettings-int-int-}
```
public LzipArchiveSettings(int dictionarySize, int maxMemberSize)
```


Initierar en ny instans av [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) med en specifik ordboksstorlek.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dictionarySize | int | ordboksstorlek för LZMA-komprimering i byte |
| maxMemberSize | int | Maximal storlek för en medlem i lzip-arkivet, angiven i byte. Standardvärdet är 60 MB. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Hämtar antalet komprimeringstrådar. Om värdet är större än 1 kommer komprimering med flera trådar att användas.

**Returns:**
int - antalet komprimeringstrådar
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Hämtar storleken på ordboken som används av LZMA-komprimering.

**Returns:**
int - storleken på ordboken som används av LZMA-komprimering
### getFastSpeed() {#getFastSpeed--}
```
public static LzipArchiveSettings getFastSpeed()
```


Hämtar en instans av klassen [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) med ordboksstorlek lika med 1 megabyte i LZMA-filter.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 1 megabyte in LZMA filter
### getFastestSpeed() {#getFastestSpeed--}
```
public static LzipArchiveSettings getFastestSpeed()
```


Hämtar en instans av klassen [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) med ordboksstorlek lika med 65536 byte i LZMA-filter.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 65536 bytes in LZMA filter
### getHighCompression() {#getHighCompression--}
```
public static LzipArchiveSettings getHighCompression()
```


Hämtar en instans av klassen [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) med ordboksstorlek lika med 32 megabyte i LZMA-filter.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 32 megabytes in LZMA filter
### getMaxMemberSize() {#getMaxMemberSize--}
```
public final long getMaxMemberSize()
```


Hämtar den maximala storleken för en medlem i lzip-arkivet, angiven i byte.

**Returns:**
long - den maximala storleken för en medlem i lzip-arkivet, angiven i byte
### getMaximumCompression() {#getMaximumCompression--}
```
public static LzipArchiveSettings getMaximumCompression()
```


Hämtar en instans av klassen [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) med ordboksstorlek lika med 64 megabyte i LZMA-filter.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 64 megabytes in LZMA filter
### getNormal() {#getNormal--}
```
public static LzipArchiveSettings getNormal()
```


Hämtar en instans av klassen [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) med ordboksstorlek lika med 16 megabyte i LZMA-filter.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 16 megabytes in LZMA filter
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Ställer in antalet komprimeringstrådar. Om värdet är större än 1 kommer komprimering med flera trådar att användas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | antal trådar för komprimering |

