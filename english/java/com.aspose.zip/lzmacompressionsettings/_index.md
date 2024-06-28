---
title: LzmaCompressionSettings
second_title: Aspose.ZIP for Java API Reference
description: Settings for LZMA compression method.
type: docs
weight: 41
url: /java/com.aspose.zip/lzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class LzmaCompressionSettings extends CompressionSettings
```

Settings for LZMA compression method.

The Lempel\\u2013Ziv\\u2013Markov chain algorithm (LZMA) is an algorithm used to perform lossless data compression. This algorithm uses a dictionary compression scheme somewhat similar to the LZ77 algorithm and features a high compression ratio and a variable compression-dictionary size.

See more: [Lempel\\u2013Ziv\\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Constructors

| Constructor | Description |
| --- | --- |
| [LzmaCompressionSettings()](#LzmaCompressionSettings--) | Initializes a new instance of the [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) class with default dictionary size, equals to 16 megabytes. |
### LzmaCompressionSettings() {#LzmaCompressionSettings--}
```
public LzmaCompressionSettings()
```


Initializes a new instance of the [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) class with default dictionary size, equals to 16 megabytes.

```

     try (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save(zipFile);
     }
 
```



