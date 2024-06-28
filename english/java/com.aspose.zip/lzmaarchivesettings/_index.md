---
title: LzmaArchiveSettings
second_title: Aspose.ZIP for Java API Reference
description: Settings for LZMA compression method within lzma archive.
type: docs
weight: 40
url: /java/com.aspose.zip/lzmaarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzmaArchiveSettings
```

Settings for LZMA compression method within lzma archive.

The Lempel\\u2013Ziv\\u2013Markov chain algorithm (LZMA) is an algorithm used to perform lossless data compression. This algorithm uses a dictionary compression scheme somewhat similar to the LZ77 algorithm and features a high compression ratio and a variable compression-dictionary size.

See more: [Lempel\\u2013Ziv\\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Constructors

| Constructor | Description |
| --- | --- |
| [LzmaArchiveSettings()](#LzmaArchiveSettings--) | Initializes a new instance of the [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) class with default dictionary size, equals to 16 megabytes. |
## Methods

| Method | Description |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data is kept in memory. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data is kept in memory. |
### LzmaArchiveSettings() {#LzmaArchiveSettings--}
```
public LzmaArchiveSettings()
```


Initializes a new instance of the [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) class with default dictionary size, equals to 16 megabytes.

```

     LzmaArchiveSettings settings = new LzmaArchiveSettings();
     settings.setDictionarySize(1048576);
     try (LzmaArchive archive = new LzmaArchive(settings)) {
         archive.setSource("data.bin");
         archive.save(lzmaFile);
     }
 
```



### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data is kept in memory. If not set, will be chosen accordingly to entry size.

The bigger the dictionary, the better the compression ratio usually is, but dictionaries bigger than the uncompressed data are waste of RAM.

**Returns:**
int - Dictionary (history buffer) size.
### setDictionarySize(int value) {#setDictionarySize-int-}
```
public final void setDictionarySize(int value)
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data is kept in memory. If not set, will be chosen accordingly to entry size.

The bigger the dictionary, the better the compression ratio usually is, but dictionaries bigger than the uncompressed data are waste of RAM.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | Dictionary (history buffer) size. |

