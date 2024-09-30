---
title: DeflateCompressionSettings
second_title: Aspose.ZIP for Java API Reference
description: Settings for Deflate compression method.
type: docs
weight: 32
url: /java/com.aspose.zip/deflatecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class DeflateCompressionSettings extends CompressionSettings
```

Settings for Deflate compression method.

Deflate is a lossless data compression algorithm that uses a combination of the LZ77 algorithm and Huffman coding.

See standard here: https://tools.ietf.org/html/rfc1951
## Constructors

| Constructor | Description |
| --- | --- |
| [DeflateCompressionSettings()](#DeflateCompressionSettings--) | Initializes a new instance of the [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings) class. |
### DeflateCompressionSettings() {#DeflateCompressionSettings--}
```
public DeflateCompressionSettings()
```


Initializes a new instance of the [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings) class.

```

    try (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings()))) {
        archive.createEntry("data.bin", "data.bin");
        archive.save(zipFile);
    }
 
```



