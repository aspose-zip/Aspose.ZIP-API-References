---
title: SevenZipLZMACompressionSettings
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 240
url: /python-net/aspose.zip.saving/sevenziplzmacompressionsettings/
---

## SevenZipLZMACompressionSettings class

Settings for LZMA compression method within 7z archive.

The SevenZipLZMACompressionSettings type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|SevenZipLZMACompressionSettings()|Initializes a new instance of the [SevenZipLZMACompressionSettings](/zip/python-net/aspose.zip.saving/sevenziplzmacompressionsettings/) class with default parameters.|
|SevenZipLZMACompressionSettings(dictionary_size, number_of_fast_bytes, literal_context_bits)|Initializes a new instance of the [SevenZipLZMACompressionSettings](/zip/python-net/aspose.zip.saving/sevenziplzmacompressionsettings/) class with specified dictionary size, number of fast bytes and number of literal context bits.|
|SevenZipLZMACompressionSettings(dictionary_size)|Initializes a new instance of the [SevenZipLZMACompressionSettings](/zip/python-net/aspose.zip.saving/sevenziplzmacompressionsettings/) class with specified dictionary size, number of fast bytes and number of literal context bits.|
## Properties
| Name | Description |
| :- | :- |
|method|Gets compression or decompression method.|
|dictionary_size|Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data is kept in memory.<br/>            If not set, will be chosen accordingly to entry size.  Must be between 4096 and 1073741824, or equal to zero for automatic detection based on entry size.|
|number_of_fast_bytes|Gets the number of bytes used for fast match searching in the LZMA algorithm.|
|literal_context_bits|Gets the number of literal context bits.|

### See Also

* namespace [aspose.zip.saving](/zip/python-net/aspose.zip.saving/)
* assembly [Aspose.Zip](/zip/python-net/)

