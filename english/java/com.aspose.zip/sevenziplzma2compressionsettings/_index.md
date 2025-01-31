---
title: SevenZipLZMA2CompressionSettings
second_title: Aspose.ZIP for Java API Reference
description: Settings for LZMA2 compression method within 7z archive.
type: docs
weight: 78
url: /java/com.aspose.zip/sevenziplzma2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMA2CompressionSettings extends SevenZipCompressionSettings
```

Settings for LZMA2 compression method within 7z archive.

LZMA2 supports multiple runs of compressed LZMA data and uncompressed data.

See more: [Lempel\\u2013Ziv\\u2013Markov\_chain\_algorithm][Lempel_u2013Ziv_u2013Markov_chain_algorithm]


[Lempel_u2013Ziv_u2013Markov_chain_algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Constructors

| Constructor | Description |
| --- | --- |
| [SevenZipLZMA2CompressionSettings()](#SevenZipLZMA2CompressionSettings--) | Instantiates settings for LZMA2 compression method within 7z archive. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize)](#SevenZipLZMA2CompressionSettings-int-) | Instantiates settings for LZMA2 compression method within 7z archive. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)](#SevenZipLZMA2CompressionSettings-int-int-) | Instantiates settings for LZMA2 compression method within 7z archive. |
## Methods

| Method | Description |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Gets compression thread count. |
| [getDictionarySize()](#getDictionarySize--) | Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data is kept in memory. |
| [getFastBytes()](#getFastBytes--) | Gets the controls number of fast bytes used by the LZMA2 compressor. |
| [getMethod()](#getMethod--) | Gets compression or decompression method. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Sets compression thread count. |
### SevenZipLZMA2CompressionSettings() {#SevenZipLZMA2CompressionSettings--}
```
public SevenZipLZMA2CompressionSettings()
```


Instantiates settings for LZMA2 compression method within 7z archive.

### SevenZipLZMA2CompressionSettings(int dictionarySize) {#SevenZipLZMA2CompressionSettings-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize)
```


Instantiates settings for LZMA2 compression method within 7z archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | size of history buffer, must be between 4096 and 1073741824.

The bigger the dictionary, the better the compression ratio usually is, but dictionaries bigger than the uncompressed data are waste of RAM. |

### SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes) {#SevenZipLZMA2CompressionSettings-int-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)
```


Instantiates settings for LZMA2 compression method within 7z archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | size of history buffer, must be between 4096 and 1073741824.

The bigger the dictionary, the better the compression ratio usually is, but dictionaries bigger than the uncompressed data are waste of RAM. |
| fastBytes | int | controls number of fast bytes used by the LZMA2 compressors. A larger number of fast bytes can provide a better compression ratio at the expense of compression speed. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Gets compression thread count. If the value greater than 1, multithreading compression will be used.

**Returns:**
int - compression thread count
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data is kept in memory.

**Returns:**
int - dictionary (history buffer) size
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


Gets the controls number of fast bytes used by the LZMA2 compressor.

**Returns:**
int - the controls number of fast bytes used by the LZMA2 compressor
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Gets compression or decompression method.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method.
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Sets compression thread count. If the value greater than 1, multithreading compression will be used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | compression thread count.

Do not set this number more than CPU cores. |

