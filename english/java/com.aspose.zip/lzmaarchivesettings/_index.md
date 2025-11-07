---
title: LzmaArchiveSettings
second_title: Aspose.ZIP for Java API Reference
description: Settings for lzma archive.
type: docs
weight: 65
url: /java/com.aspose.zip/lzmaarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzmaArchiveSettings
```

Settings for lzma archive.

The Lempel\\u2013Ziv\\u2013Markov chain algorithm (LZMA) is an algorithm used to perform lossless data compression. This algorithm uses a dictionary compression scheme somewhat similar to the LZ77 algorithm and features a high compression ratio and a variable compression-dictionary size.

See more: [Lempel\\u2013Ziv\\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Constructors

| Constructor | Description |
| --- | --- |
| [LzmaArchiveSettings()](#LzmaArchiveSettings--) | Initializes a new instance of the [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) class with default dictionary size, equals to 16 megabytes, number of fast bytes equal to 32 and literal context bits equal to 3. |
## Methods

| Method | Description |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | Gets an event that is raised when a portion of raw stream compressed. |
| [getDictionarySize()](#getDictionarySize--) | Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Gets the number of literal context bits. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Gets the number of bytes used for fast match searching in the LZMA algorithm. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Sets an event that is raised when a portion of raw stream compressed. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory. |
| [setLiteralContextBits(int value)](#setLiteralContextBits-int-) | Sets the number of literal context bits. |
| [setNumberOfFastBytes(int value)](#setNumberOfFastBytes-int-) | Sets the number of bytes used for fast match searching in the LZMA algorithm. |
### LzmaArchiveSettings() {#LzmaArchiveSettings--}
```
public LzmaArchiveSettings()
```


Initializes a new instance of the [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) class with default dictionary size, equals to 16 megabytes, number of fast bytes equal to 32 and literal context bits equal to 3.

```

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


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory. If not set, will be chosen accordingly to entry size.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM.

**Returns:**
int - Dictionary (history buffer) size.
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
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

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

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM.

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

