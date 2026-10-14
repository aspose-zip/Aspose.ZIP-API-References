---
title: "LzmaArchiveSettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "lzma 存档的设置。"
type: docs
weight: 87
url: /zh/java/com.aspose.zip/lzmaarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzmaArchiveSettings
```

lzma 存档的设置。

Lempel‑Ziv‑Markov 链算法（LZMA）是一种用于实现无损数据压缩的算法。该算法使用一种与 LZ77 算法略有相似的字典压缩方案，具有高压缩率和可变的压缩字典大小。

查看更多：[Lempel\u2013Ziv\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [LzmaArchiveSettings()](#LzmaArchiveSettings--) | 初始化 [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) 类的新实例，默认字典大小为 16 兆字节，快速字节数为 32，文字上下文位数为 3。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | 获取在原始流的一部分被压缩时触发的事件。 |
| [getDictionarySize()](#getDictionarySize--) | 字典（历史缓冲区）大小表示最近处理的未压缩数据在内存中保留的字节数。 |
| [getLiteralContextBits()](#getLiteralContextBits--) | 获取文字上下文位的数量。 |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | 获取 LZMA 算法中用于快速匹配搜索的字节数。 |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | 设置在原始流的一部分被压缩时触发的事件。 |
| [setDictionarySize(int value)](#setDictionarySize-int-) | 字典（历史缓冲区）大小表示最近处理的未压缩数据在内存中保留的字节数。 |
| [setLiteralContextBits(int value)](#setLiteralContextBits-int-) | 设置文字上下文位的数量。 |
| [setNumberOfFastBytes(int value)](#setNumberOfFastBytes-int-) | 设置 LZMA 算法中用于快速匹配搜索的字节数。 |
### LzmaArchiveSettings() {#LzmaArchiveSettings--}
```
public LzmaArchiveSettings()
```


初始化 [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) 类的新实例，默认字典大小为 16 兆字节，快速字节数为 32，文字上下文位数为 3。

```

``````

LzmaArchiveSettings settings = new LzmaArchiveSettings();
settings.setDictionarySize(1048576);
try (LzmaArchive archive = new LzmaArchive(settings)) {
archive.setSource("data.bin");
archive.save(lzmaFile);
}
 
```



### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Gets an event that is raised when a portion of raw stream compressed.

```

``````

    lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```



**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


字典（历史缓冲区）大小表示最近处理的未压缩数据在内存中保留的字节数。如果未设置，将根据条目大小自动选择。

字典越大，通常压缩率越好——但大于未压缩数据的字典会浪费 RAM。LZMA 压缩包的字典大小必须是二的幂 (2^n) 或二的幂的三倍 (3\*2^n)。

**Returns:**
int - 字典（历史缓冲区）大小。
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


获取文字上下文位的数量。

文字上下文位定义了使用前一个未压缩字节的最高有效位来预测下一个文字字节的位数。取值范围为 0 到 8。

**Returns:**
int - 文字上下文位的数量。
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


获取 LZMA 算法中用于快速匹配搜索的字节数。

更高的值允许压缩器搜索更长的匹配，这可以略微提升压缩率，但会减慢压缩速度。

**Returns:**
int - 用于 LZMA 算法中快速匹配搜索的字节数。
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


设置在原始流的一部分被压缩时触发的事件。

```

``````

lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when a portion of raw stream compressed |

### setDictionarySize(int value) {#setDictionarySize-int-}
```
public final void setDictionarySize(int value)
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory. If not set, will be chosen accordingly to entry size.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM. The disctionary size of LZMA archive must be either a power of two (2^n) or three times a power of two (3\*2^n).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | Dictionary (history buffer) size. |

### setLiteralContextBits(int value) {#setLiteralContextBits-int-}
```
public final void setLiteralContextBits(int value)
```


Sets the number of literal context bits.

Literal Context Bits define how many of the most significant bits of the previous uncompressed byte are used to predict the bits of the next literal byte. Must be from 0 to 8.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of literal context bits. |

### setNumberOfFastBytes(int value) {#setNumberOfFastBytes-int-}
```
public final void setNumberOfFastBytes(int value)
```


Sets the number of bytes used for fast match searching in the LZMA algorithm.

A higher value allows the compressor to search longer matches, which can improve the compression ratio slightly but slows down compression.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of bytes used for fast match searching in the LZMA algorithm. |

