---
title: "Lz4ArchiveSetting"
second_title: "Aspose.ZIP for Java API 参考"
description: "LZ4 存档组成的设置。"
type: docs
weight: 81
url: /zh/java/com.aspose.zip/lz4archivesetting/
---

**Inheritance:**
java.lang.Object
```
public class Lz4ArchiveSetting
```

LZ4 存档组成的设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Lz4ArchiveSetting()](#Lz4ArchiveSetting--) | 使用默认参数初始化 [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getIncludeBlockChecksum()](#getIncludeBlockChecksum--) | 获取一个值，指示是否在压缩块的末尾包含压缩的 xxh32 哈希。 |
| [getIncludeContentChecksum()](#getIncludeContentChecksum--) | 获取一个值，指示是否在 LZ4 存档的末尾包含内容 xxh32 哈希。 |
| [getIncludeContentSize()](#getIncludeContentSize--) | 获取一个值，指示是否在帧中包含内容大小。 |
| [setIncludeBlockChecksum(boolean value)](#setIncludeBlockChecksum-boolean-) | 设置一个值，指示是否在压缩块的末尾包含压缩的 xxh32 哈希。 |
| [setIncludeContentChecksum(boolean value)](#setIncludeContentChecksum-boolean-) | 设置一个值，指示是否在 LZ4 存档的末尾包含内容 xxh32 哈希。 |
| [setIncludeContentSize(boolean value)](#setIncludeContentSize-boolean-) | 设置一个值，指示是否在帧中包含内容大小。 |
### Lz4ArchiveSetting() {#Lz4ArchiveSetting--}
```
public Lz4ArchiveSetting()
```


使用默认参数初始化 [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) 类的新实例。

### getIncludeBlockChecksum() {#getIncludeBlockChecksum--}
```
public final boolean getIncludeBlockChecksum()
```


获取一个值，指示是否在压缩块的末尾包含压缩的 xxh32 哈希。

默认值为 false。

**Returns:**
boolean - 指示是否在压缩块的末尾包含压缩的 xxh32 哈希的值。
### getIncludeContentChecksum() {#getIncludeContentChecksum--}
```
public final boolean getIncludeContentChecksum()
```


获取一个值，指示是否在 LZ4 存档的末尾包含内容 xxh32 哈希。

默认值为 true。

**Returns:**
布尔 - 一个指示是否在 LZ4 存档末尾包含内容 xxh32 哈希的值。
### getIncludeContentSize() {#getIncludeContentSize--}
```
public final boolean getIncludeContentSize()
```


获取一个值，指示是否在帧中包含内容大小。

默认值为 false。适用于源流可定位时。

**Returns:**
布尔 - 一个指示是否在帧中包含内容大小的值。
### setIncludeBlockChecksum(boolean value) {#setIncludeBlockChecksum-boolean-}
```
public final void setIncludeBlockChecksum(boolean value)
```


设置一个值，指示是否在压缩块的末尾包含压缩的 xxh32 哈希。

默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 布尔 | 一个指示是否在压缩块末尾包含压缩的 xxh32 哈希的值。 |

### setIncludeContentChecksum(boolean value) {#setIncludeContentChecksum-boolean-}
```
public final void setIncludeContentChecksum(boolean value)
```


设置一个值，指示是否在 LZ4 存档的末尾包含内容 xxh32 哈希。

默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 布尔 | 一个指示是否在 LZ4 存档末尾包含内容 xxh32 哈希的值。 |

### setIncludeContentSize(boolean value) {#setIncludeContentSize-boolean-}
```
public final void setIncludeContentSize(boolean value)
```


设置一个值，指示是否在帧中包含内容大小。

默认值为 false。适用于源流可定位时。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 布尔 | 一个指示是否在帧中包含内容大小的值。 |

