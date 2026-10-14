---
title: "SevenZipLZMA2CompressionSettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "7z 存档中 LZMA2 压缩方法的设置。"
type: docs
weight: 114
url: /zh/java/com.aspose.zip/sevenziplzma2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMA2CompressionSettings extends SevenZipCompressionSettings
```

7z 存档中 LZMA2 压缩方法的设置。

LZMA2 支持多次压缩的 LZMA 数据和未压缩数据。

查看更多： [Lempel\\u2013Ziv\\u2013Markov\_chain\_algorithm][Lempel_u2013Ziv_u2013Markov_chain_algorithm]


[Lempel_u2013Ziv_u2013Markov_chain_algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [SevenZipLZMA2CompressionSettings()](#SevenZipLZMA2CompressionSettings--) | 在 7z 存档中实例化 LZMA2 压缩方法的设置。 |
| [SevenZipLZMA2CompressionSettings(int dictionarySize)](#SevenZipLZMA2CompressionSettings-int-) | 在 7z 存档中实例化 LZMA2 压缩方法的设置。 |
| [SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)](#SevenZipLZMA2CompressionSettings-int-int-) | 在 7z 存档中实例化 LZMA2 压缩方法的设置。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | 获取压缩线程数。 |
| [getDictionarySize()](#getDictionarySize--) | 字典（历史缓冲区）大小表示最近处理的未压缩数据在内存中保留的字节数。 |
| [getFastBytes()](#getFastBytes--) | 获取 LZMA2 压缩器使用的快速字节控制数。 |
| [getMethod()](#getMethod--) | 获取压缩或解压缩方法。 |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | 设置压缩线程数。 |
### SevenZipLZMA2CompressionSettings() {#SevenZipLZMA2CompressionSettings--}
```
public SevenZipLZMA2CompressionSettings()
```


在 7z 存档中实例化 LZMA2 压缩方法的设置。

### SevenZipLZMA2CompressionSettings(int dictionarySize) {#SevenZipLZMA2CompressionSettings-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize)
```


在 7z 存档中实例化 LZMA2 压缩方法的设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | dictionarySize | int | 历史缓冲区的大小，必须在 4096 到 1073741824 之间。 |

字典越大，通常压缩比越好——但大于未压缩数据的字典会浪费 RAM。 |

### SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes) {#SevenZipLZMA2CompressionSettings-int-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)
```


在 7z 存档中实例化 LZMA2 压缩方法的设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | dictionarySize | int | 历史缓冲区的大小，必须在 4096 到 1073741824 之间。 |

字典越大，通常压缩比越好——但大于未压缩数据的字典会浪费 RAM。 |
| fastBytes | int | 控制 LZMA2 压缩器使用的快速字节数量。更多的快速字节可以在牺牲压缩速度的情况下提供更好的压缩比。 |

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


字典（历史缓冲区）大小表示最近处理的未压缩数据在内存中保留的字节数。

**Returns:**
int - 字典（历史缓冲区）大小
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


获取 LZMA2 压缩器使用的快速字节控制数。

**Returns:**
int - LZMA2 压缩器使用的快速字节控制数
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


获取压缩或解压缩方法。

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method.
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


设置压缩线程数。如果该值大于 1，将使用多线程压缩。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 压缩线程数。 |

不要将此数字设置超过 CPU 核心数。 |

