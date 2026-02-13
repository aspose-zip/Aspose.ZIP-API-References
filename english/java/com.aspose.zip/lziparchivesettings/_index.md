---
title: LzipArchiveSettings
second_title: Aspose.ZIP for Java API Reference
description: The class contains setting of a particular lzip archive.
type: docs
weight: 67
url: /java/com.aspose.zip/lziparchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzipArchiveSettings
```

The class contains setting of a particular lzip archive.
## Constructors

| Constructor | Description |
| --- | --- |
| [LzipArchiveSettings(int dictionarySize)](#LzipArchiveSettings-int-) | Initializes a new instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) with particular dictionary size. |
| [LzipArchiveSettings(int dictionarySize, int maxMemberSize)](#LzipArchiveSettings-int-int-) | Initializes a new instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) with particular dictionary size. |
## Methods

| Method | Description |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Gets compression thread count. |
| [getDictionarySize()](#getDictionarySize--) | Gets the size of dictionary which used by LZMA compression. |
| [getFastSpeed()](#getFastSpeed--) | Gets the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 1 megabyte in LZMA filter. |
| [getFastestSpeed()](#getFastestSpeed--) | Gets the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 65536 bytes in LZMA filter. |
| [getHighCompression()](#getHighCompression--) | Gets the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 32 megabytes in LZMA filter. |
| [getMaxMemberSize()](#getMaxMemberSize--) | Gets the maximum size of one member in lzip archive presented in bytes. |
| [getMaximumCompression()](#getMaximumCompression--) | Gets the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 64 megabytes in LZMA filter. |
| [getNormal()](#getNormal--) | Gets the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 16 megabytes in LZMA filter. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Sets compression thread count. |
### LzipArchiveSettings(int dictionarySize) {#LzipArchiveSettings-int-}
```
public LzipArchiveSettings(int dictionarySize)
```


Initializes a new instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) with particular dictionary size.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | dictionary size for LZMA compression in bytes |

### LzipArchiveSettings(int dictionarySize, int maxMemberSize) {#LzipArchiveSettings-int-int-}
```
public LzipArchiveSettings(int dictionarySize, int maxMemberSize)
```


Initializes a new instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) with particular dictionary size.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | dictionary size for LZMA compression in bytes |
| maxMemberSize | int | Maximum size of one member in lzip archive presented in bytes. The default value is 60 MB. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Gets compression thread count. If the value is greater than 1, multithreading compression will be used.

**Returns:**
int - compression thread count
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Gets the size of dictionary which used by LZMA compression.

**Returns:**
int - the size of dictionary which used by LZMA compression
### getFastSpeed() {#getFastSpeed--}
```
public static LzipArchiveSettings getFastSpeed()
```


Gets the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 1 megabyte in LZMA filter.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 1 megabyte in LZMA filter
### getFastestSpeed() {#getFastestSpeed--}
```
public static LzipArchiveSettings getFastestSpeed()
```


Gets the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 65536 bytes in LZMA filter.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 65536 bytes in LZMA filter
### getHighCompression() {#getHighCompression--}
```
public static LzipArchiveSettings getHighCompression()
```


Gets the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 32 megabytes in LZMA filter.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 32 megabytes in LZMA filter
### getMaxMemberSize() {#getMaxMemberSize--}
```
public final long getMaxMemberSize()
```


Gets the maximum size of one member in lzip archive presented in bytes.

**Returns:**
long - the maximum size of one member in lzip archive presented in bytes
### getMaximumCompression() {#getMaximumCompression--}
```
public static LzipArchiveSettings getMaximumCompression()
```


Gets the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 64 megabytes in LZMA filter.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 64 megabytes in LZMA filter
### getNormal() {#getNormal--}
```
public static LzipArchiveSettings getNormal()
```


Gets the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 16 megabytes in LZMA filter.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 16 megabytes in LZMA filter
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Sets compression thread count. If the value is greater than 1, multithreading compression will be used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | compression thread count |

