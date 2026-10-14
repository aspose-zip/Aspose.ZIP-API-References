---
title: "LzipArchiveSettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Die Klasse enthält Einstellungen eines bestimmten Lzip-Archivs."
type: docs
weight: 84
url: /de/java/com.aspose.zip/lziparchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzipArchiveSettings
```

Die Klasse enthält Einstellungen eines bestimmten Lzip-Archivs.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [LzipArchiveSettings(int dictionarySize)](#LzipArchiveSettings-int-) | Initialisiert eine neue Instanz von [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) mit einer bestimmten Wörterbuchgröße. |
| [LzipArchiveSettings(int dictionarySize, int maxMemberSize)](#LzipArchiveSettings-int-int-) | Initialisiert eine neue Instanz von [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) mit einer bestimmten Wörterbuchgröße. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Liefert die Anzahl der Komprimierungs-Threads. |
| [getDictionarySize()](#getDictionarySize--) | Gibt die Größe des Wörterbuchs zurück, das von der LZMA-Kompression verwendet wird. |
| [getFastSpeed()](#getFastSpeed--) | Gibt die Instanz der Klasse [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) zurück, bei der die Wörterbuchgröße im LZMA-Filter 1 Megabyte beträgt. |
| [getFastestSpeed()](#getFastestSpeed--) | Gibt die Instanz der Klasse [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) zurück, bei der die Wörterbuchgröße im LZMA-Filter 65536 Bytes beträgt. |
| [getHighCompression()](#getHighCompression--) | Gibt die Instanz der Klasse [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) zurück, bei der die Wörterbuchgröße im LZMA-Filter 32 Megabyte beträgt. |
| [getMaxMemberSize()](#getMaxMemberSize--) | Gibt die maximale Größe eines Elements im Lzip-Archiv in Bytes zurück. |
| [getMaximumCompression()](#getMaximumCompression--) | Gibt die Instanz der Klasse [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) zurück, bei der die Wörterbuchgröße im LZMA-Filter 64 Megabyte beträgt. |
| [getNormal()](#getNormal--) | Gibt die Instanz der Klasse [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) zurück, bei der die Wörterbuchgröße im LZMA-Filter 16 Megabyte beträgt. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Setzt die Anzahl der Komprimierungs-Threads. |
### LzipArchiveSettings(int dictionarySize) {#LzipArchiveSettings-int-}
```
public LzipArchiveSettings(int dictionarySize)
```


Initialisiert eine neue Instanz von [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) mit einer bestimmten Wörterbuchgröße.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dictionarySize | int | Wörterbuchgröße für LZMA-Kompression in Bytes |

### LzipArchiveSettings(int dictionarySize, int maxMemberSize) {#LzipArchiveSettings-int-int-}
```
public LzipArchiveSettings(int dictionarySize, int maxMemberSize)
```


Initialisiert eine neue Instanz von [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) mit einer bestimmten Wörterbuchgröße.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dictionarySize | int | Wörterbuchgröße für LZMA-Kompression in Bytes |
| maxMemberSize | int | Maximale Größe eines Elements im Lzip-Archiv in Bytes. Der Standardwert beträgt 60 MB. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Gibt die Anzahl der Kompressionsthreads zurück. Wenn der Wert größer als 1 ist, wird eine Multithread-Kompression verwendet.

**Returns:**
int - Anzahl der Kompressionsthreads
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Gibt die Größe des Wörterbuchs zurück, das von der LZMA-Kompression verwendet wird.

**Returns:**
int - Größe des Wörterbuchs, das von der LZMA-Kompression verwendet wird
### getFastSpeed() {#getFastSpeed--}
```
public static LzipArchiveSettings getFastSpeed()
```


Gibt die Instanz der Klasse [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) zurück, bei der die Wörterbuchgröße im LZMA-Filter 1 Megabyte beträgt.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 1 megabyte in LZMA filter
### getFastestSpeed() {#getFastestSpeed--}
```
public static LzipArchiveSettings getFastestSpeed()
```


Gibt die Instanz der Klasse [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) zurück, bei der die Wörterbuchgröße im LZMA-Filter 65536 Bytes beträgt.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 65536 bytes in LZMA filter
### getHighCompression() {#getHighCompression--}
```
public static LzipArchiveSettings getHighCompression()
```


Gibt die Instanz der Klasse [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) zurück, bei der die Wörterbuchgröße im LZMA-Filter 32 Megabyte beträgt.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 32 megabytes in LZMA filter
### getMaxMemberSize() {#getMaxMemberSize--}
```
public final long getMaxMemberSize()
```


Gibt die maximale Größe eines Elements im Lzip-Archiv in Bytes zurück.

**Returns:**
long - maximale Größe eines Elements im Lzip-Archiv in Bytes
### getMaximumCompression() {#getMaximumCompression--}
```
public static LzipArchiveSettings getMaximumCompression()
```


Gibt die Instanz der Klasse [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) zurück, bei der die Wörterbuchgröße im LZMA-Filter 64 Megabyte beträgt.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 64 megabytes in LZMA filter
### getNormal() {#getNormal--}
```
public static LzipArchiveSettings getNormal()
```


Gibt die Instanz der Klasse [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) zurück, bei der die Wörterbuchgröße im LZMA-Filter 16 Megabyte beträgt.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 16 megabytes in LZMA filter
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Setzt die Anzahl der Komprimierungs-Threads. Wenn der Wert größer als 1 ist, wird eine mehrthreadige Komprimierung verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Komprimierungs-Thread-Anzahl |

