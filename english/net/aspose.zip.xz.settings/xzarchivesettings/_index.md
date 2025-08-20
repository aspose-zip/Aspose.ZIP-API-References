---
title: Class XzArchiveSettings
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Xz.Settings.XzArchiveSettings class. The class contains a set of setting particular xz archive
type: docs
weight: 1210
url: /net/aspose.zip.xz.settings/xzarchivesettings/
---
## XzArchiveSettings class

The class contains a set of setting particular xz archive.

```csharp
public class XzArchiveSettings
```

## Constructors

| Name | Description |
| --- | --- |
| [XzArchiveSettings](xzarchivesettings/#constructor)() | Initializes a new instance of the `XzArchiveSettings` class using single LZMA2 compression. |
| [XzArchiveSettings](xzarchivesettings/#constructor_1)(XzFilterSettings[], long, XzCheckType) | Initializes a new instance of the `XzArchiveSettings` class with custom parameters. |

## Properties

| Name | Description |
| --- | --- |
| static [FastestSpeed](../../aspose.zip.xz.settings/xzarchivesettings/fastestspeed/) { get; } | Gets the instance of the `XzArchiveSettings` class with dictionary size equals to 65536 bytes in LZMA2 filter, block size equals to 1 megabyte and CRC32 checksum. |
| static [FastSpeed](../../aspose.zip.xz.settings/xzarchivesettings/fastspeed/) { get; } | Gets the instance of the `XzArchiveSettings` class with dictionary size equals to 1 megabyte in LZMA2 filter, block size equals to 4 megabytes and CRC32 checksum. |
| static [HighCompression](../../aspose.zip.xz.settings/xzarchivesettings/highcompression/) { get; } | Gets the instance of the `XzArchiveSettings` class with dictionary size equals to 32 megabytes in LZMA2 filter, block size equals to 128 megabytes and CRC32 checksum. |
| static [MaximumCompression](../../aspose.zip.xz.settings/xzarchivesettings/maximumcompression/) { get; } | Gets the instance of the `XzArchiveSettings` class with dictionary size equals to 64 megabytes in LZMA2 filter, block size equals to 256 megabytes and CRC32 checksum. |
| static [Normal](../../aspose.zip.xz.settings/xzarchivesettings/normal/) { get; } | Gets the instance of the `XzArchiveSettings` class with dictionary size equals to 16 megabytes in LZMA2 filter, block size equals to 64 megabytes and CRC32 checksum. |
| [CompressionThreads](../../aspose.zip.xz.settings/xzarchivesettings/compressionthreads/) { get; set; } | Gets or sets compression thread count. If the value is greater than 1, multithreading compression will be used. |

### See Also

* namespace [Aspose.Zip.Xz.Settings](../../aspose.zip.xz.settings/)
* assembly [Aspose.Zip](../../)


