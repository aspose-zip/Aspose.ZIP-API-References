---
title: "LzipArchiveSettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "该类包含特定 lzip 存档的设置。"
type: docs
weight: 84
url: /zh/java/com.aspose.zip/lziparchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzipArchiveSettings
```

该类包含特定 lzip 存档的设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [LzipArchiveSettings(int dictionarySize)](#LzipArchiveSettings-int-) | 使用特定字典大小初始化 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 的新实例。 |
| [LzipArchiveSettings(int dictionarySize, int maxMemberSize)](#LzipArchiveSettings-int-int-) | 使用特定字典大小初始化 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | 获取压缩线程数。 |
| [getDictionarySize()](#getDictionarySize--) | 获取 LZMA 压缩使用的字典大小。 |
| [getFastSpeed()](#getFastSpeed--) | 获取在 LZMA 过滤器中字典大小等于 1 兆字节的 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 类实例。 |
| [getFastestSpeed()](#getFastestSpeed--) | 获取在 LZMA 过滤器中字典大小等于 65536 字节的 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 类实例。 |
| [getHighCompression()](#getHighCompression--) | 获取在 LZMA 过滤器中字典大小等于 32 兆字节的 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 类实例。 |
| [getMaxMemberSize()](#getMaxMemberSize--) | 获取 lzip 存档中单个成员的最大大小（以字节为单位）。 |
| [getMaximumCompression()](#getMaximumCompression--) | 获取在 LZMA 过滤器中字典大小等于 64 兆字节的 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 类实例。 |
| [getNormal()](#getNormal--) | 获取在 LZMA 过滤器中字典大小等于 16 兆字节的 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 类实例。 |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | 设置压缩线程数。 |
### LzipArchiveSettings(int dictionarySize) {#LzipArchiveSettings-int-}
```
public LzipArchiveSettings(int dictionarySize)
```


使用特定字典大小初始化 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dictionarySize | int | LZMA 压缩的字典大小（字节） |

### LzipArchiveSettings(int dictionarySize, int maxMemberSize) {#LzipArchiveSettings-int-int-}
```
public LzipArchiveSettings(int dictionarySize, int maxMemberSize)
```


使用特定字典大小初始化 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dictionarySize | int | LZMA 压缩的字典大小（字节） |
| maxMemberSize | int | lzip 存档中单个成员的最大大小（字节）。默认值为 60 MB。 |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


获取压缩线程数。如果该值大于 1，将使用多线程压缩。

**Returns:**
int - 压缩线程数
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


获取 LZMA 压缩使用的字典大小。

**Returns:**
int - LZMA 压缩使用的字典大小
### getFastSpeed() {#getFastSpeed--}
```
public static LzipArchiveSettings getFastSpeed()
```


获取在 LZMA 过滤器中字典大小等于 1 兆字节的 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 类实例。

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 1 megabyte in LZMA filter
### getFastestSpeed() {#getFastestSpeed--}
```
public static LzipArchiveSettings getFastestSpeed()
```


获取在 LZMA 过滤器中字典大小等于 65536 字节的 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 类实例。

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 65536 bytes in LZMA filter
### getHighCompression() {#getHighCompression--}
```
public static LzipArchiveSettings getHighCompression()
```


获取在 LZMA 过滤器中字典大小等于 32 兆字节的 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 类实例。

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 32 megabytes in LZMA filter
### getMaxMemberSize() {#getMaxMemberSize--}
```
public final long getMaxMemberSize()
```


获取 lzip 存档中单个成员的最大大小（以字节为单位）。

**Returns:**
long - lzip 存档中单个成员的最大大小（字节）
### getMaximumCompression() {#getMaximumCompression--}
```
public static LzipArchiveSettings getMaximumCompression()
```


获取在 LZMA 过滤器中字典大小等于 64 兆字节的 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 类实例。

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 64 megabytes in LZMA filter
### getNormal() {#getNormal--}
```
public static LzipArchiveSettings getNormal()
```


获取在 LZMA 过滤器中字典大小等于 16 兆字节的 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 类实例。

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 16 megabytes in LZMA filter
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


设置压缩线程数。如果该值大于 1，将使用多线程压缩。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 压缩线程计数 |

