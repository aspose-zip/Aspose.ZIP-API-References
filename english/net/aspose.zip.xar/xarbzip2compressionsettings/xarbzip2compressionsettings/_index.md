---
title: XarBzip2CompressionSettings.XarBzip2CompressionSettings
second_title: Aspose.ZIP for .NET API Reference
description: XarBzip2CompressionSettings constructor. Initializes a new instance of the XarBzip2CompressionSettings class
type: docs
weight: 10
url: /net/aspose.zip.xar/xarbzip2compressionsettings/xarbzip2compressionsettings/
---
## XarBzip2CompressionSettings(int) {#constructor_1}

Initializes a new instance of the [`XarBzip2CompressionSettings`](../) class.

```csharp
public XarBzip2CompressionSettings(int blockSize)
```

| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | Int32 | Block size in hundreds of kilobytes. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | Block size is not between 1 and 9. |

## Examples

```csharp
using (XarArchive archive = new XarArchive())
{
    archive.CreateEntry("data.bin", "data.bin", new XarBzip2CompressionSettings(1));
    archive.Save("archive.xar");
}
```

### See Also

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## XarBzip2CompressionSettings() {#constructor}

Initializes a new instance of the [`XarBzip2CompressionSettings`](../) class with default block size, equals to 9 hundred of kilobytes.

```csharp
public XarBzip2CompressionSettings()
```

### See Also

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)


