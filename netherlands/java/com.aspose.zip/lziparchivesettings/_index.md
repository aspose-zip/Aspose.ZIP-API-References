---
title: "LzipArchiveSettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "De klasse bevat instellingen van een specifiek lzip-archief."
type: docs
weight: 84
url: /nl/java/com.aspose.zip/lziparchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzipArchiveSettings
```

De klasse bevat instellingen van een specifiek lzip-archief.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [LzipArchiveSettings(int dictionarySize)](#LzipArchiveSettings-int-) | Initialiseert een nieuw exemplaar van de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) met een specifieke woordenboekgrootte. |
| [LzipArchiveSettings(int dictionarySize, int maxMemberSize)](#LzipArchiveSettings-int-int-) | Initialiseert een nieuw exemplaar van de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) met een specifieke woordenboekgrootte. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Haalt het aantal compressiedraden op. |
| [getDictionarySize()](#getDictionarySize--) | Haalt de grootte van het woordenboek op dat wordt gebruikt door LZMA-compressie. |
| [getFastSpeed()](#getFastSpeed--) | Haalt de instantie van de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) klasse op met een woordenboekgrootte van 1 megabyte in het LZMA-filter. |
| [getFastestSpeed()](#getFastestSpeed--) | Haalt de instantie van de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) klasse op met een woordenboekgrootte van 65536 bytes in het LZMA-filter. |
| [getHighCompression()](#getHighCompression--) | Haalt de instantie van de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) klasse op met een woordenboekgrootte van 32 megabyte in het LZMA-filter. |
| [getMaxMemberSize()](#getMaxMemberSize--) | Haalt de maximale grootte van één lid in een lzip-archief op, weergegeven in bytes. |
| [getMaximumCompression()](#getMaximumCompression--) | Haalt de instantie van de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) klasse op met een woordenboekgrootte van 64 megabyte in het LZMA-filter. |
| [getNormal()](#getNormal--) | Haalt de instantie van de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) klasse op met een woordenboekgrootte van 16 megabyte in het LZMA-filter. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Stelt het aantal compressiedraden in. |
### LzipArchiveSettings(int dictionarySize) {#LzipArchiveSettings-int-}
```
public LzipArchiveSettings(int dictionarySize)
```


Initialiseert een nieuw exemplaar van de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) met een specifieke woordenboekgrootte.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dictionarySize | int | woordenboekgrootte voor LZMA-compressie in bytes |

### LzipArchiveSettings(int dictionarySize, int maxMemberSize) {#LzipArchiveSettings-int-int-}
```
public LzipArchiveSettings(int dictionarySize, int maxMemberSize)
```


Initialiseert een nieuw exemplaar van de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) met een specifieke woordenboekgrootte.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dictionarySize | int | woordenboekgrootte voor LZMA-compressie in bytes |
| maxMemberSize | int | Maximale grootte van één lid in een lzip-archief, weergegeven in bytes. De standaardwaarde is 60 MB. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Haalt het aantal compressiedraden op. Als de waarde groter is dan 1, wordt multithread-compressie gebruikt.

**Returns:**
int - aantal compressiedraden
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Haalt de grootte van het woordenboek op dat wordt gebruikt door LZMA-compressie.

**Returns:**
int - de grootte van het woordenboek dat wordt gebruikt door LZMA-compressie
### getFastSpeed() {#getFastSpeed--}
```
public static LzipArchiveSettings getFastSpeed()
```


Haalt de instantie van de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) klasse op met een woordenboekgrootte van 1 megabyte in het LZMA-filter.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 1 megabyte in LZMA filter
### getFastestSpeed() {#getFastestSpeed--}
```
public static LzipArchiveSettings getFastestSpeed()
```


Haalt de instantie van de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) klasse op met een woordenboekgrootte van 65536 bytes in het LZMA-filter.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 65536 bytes in LZMA filter
### getHighCompression() {#getHighCompression--}
```
public static LzipArchiveSettings getHighCompression()
```


Haalt de instantie van de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) klasse op met een woordenboekgrootte van 32 megabyte in het LZMA-filter.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 32 megabytes in LZMA filter
### getMaxMemberSize() {#getMaxMemberSize--}
```
public final long getMaxMemberSize()
```


Haalt de maximale grootte van één lid in een lzip-archief op, weergegeven in bytes.

**Returns:**
long - de maximale grootte van één lid in een lzip-archief, weergegeven in bytes
### getMaximumCompression() {#getMaximumCompression--}
```
public static LzipArchiveSettings getMaximumCompression()
```


Haalt de instantie van de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) klasse op met een woordenboekgrootte van 64 megabyte in het LZMA-filter.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 64 megabytes in LZMA filter
### getNormal() {#getNormal--}
```
public static LzipArchiveSettings getNormal()
```


Haalt de instantie van de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) klasse op met een woordenboekgrootte van 16 megabyte in het LZMA-filter.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 16 megabytes in LZMA filter
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Stelt het aantal compressiedraden in. Als de waarde groter is dan 1, wordt multithread-compressie gebruikt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | aantal compressiedraden |

