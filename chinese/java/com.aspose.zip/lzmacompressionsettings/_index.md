---
title: "LzmaCompressionSettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "LZMA 压缩方法的设置。"
type: docs
weight: 88
url: /zh/java/com.aspose.zip/lzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class LzmaCompressionSettings extends CompressionSettings
```

LZMA 压缩方法的设置。

Lempel‑Ziv‑Markov 链算法（LZMA）是一种用于实现无损数据压缩的算法。该算法使用一种与 LZ77 算法略有相似的字典压缩方案，具有高压缩率和可变的压缩字典大小。

查看更多：[Lempel\u2013Ziv\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [LzmaCompressionSettings()](#LzmaCompressionSettings--) | 使用默认参数初始化 [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) 类的新实例。 |
| [LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)](#LzmaCompressionSettings-int-int-int-) | 使用指定的字典大小、快速字节数和文字上下文位数初始化 [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) 类的新实例。 |
| [LzmaCompressionSettings(int dictionarySize)](#LzmaCompressionSettings-int-) | 使用指定的字典大小、默认的快速字节数（32）和文字上下文位数（3）初始化 [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | 字典（历史缓冲区）大小表示最近处理的未压缩数据在内存中保留的字节数。 |
| [getLiteralContextBits()](#getLiteralContextBits--) | 获取文字上下文位的数量。 |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | 获取 LZMA 算法中用于快速匹配搜索的字节数。 |
### LzmaCompressionSettings() {#LzmaCompressionSettings--}
```
public LzmaCompressionSettings()
```


使用默认参数初始化 [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) 类的新实例。

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



### LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits) {#LzmaCompressionSettings-int-int-int-}
```
public LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)
```


Initializes a new instance of the [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) class with specified dictionary size, number of fast bytes and number of literal context bits.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824. |
| numberOfFastBytes | int | The number of bytes used for fast match searching in the LZMA algorithm. Can be in the range from 5 to 273. |
| literalContextBits | int | Sets the number of literal context bits (high bits of previous literal). It can be in range from 0 to 8. |

### LzmaCompressionSettings(int dictionarySize) {#LzmaCompressionSettings-int-}
```
public LzmaCompressionSettings(int dictionarySize)
```


Initializes a new instance of the [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) class with specified dictionary size, default number of fast bytes equal to 32 and number of literal context bits equal to 3.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824. |

### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM.

**Returns:**
int - how many bytes of the recently processed uncompressed data are kept in memory.
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


Gets the number of literal context bits.

Literal Context Bits define how many of the most significant bits of the previous uncompressed byte are used to predict the bits of the next literal byte. Must be from 0 to 8.

**Returns:**
int - the number of literal context bits.
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


Gets the number of bytes used for fast match searching in the LZMA algorithm.

A higher value allows the compressor to search longer matches, which can improve the compression ratio slightly but slows down compression.

**Returns:**
int - the number of bytes used for fast match searching in the LZMA algorithm.
