---
title: Bzip2CompressionSettings.Bzip2CompressionSettings
second_title: Aspose.ZIP for .NET API Reference
description: Bzip2CompressionSettings constructor. Initializes a new instance of the Bzip2CompressionSettings class
type: docs
weight: 10
url: /net/aspose.zip.saving/bzip2compressionsettings/bzip2compressionsettings/
---
## Bzip2CompressionSettings(int) {#constructor_1}

Initializes a new instance of the [`Bzip2CompressionSettings`](../) class.

```csharp
public Bzip2CompressionSettings(int blockSize)
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
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### See Also

* class [Bzip2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## Bzip2CompressionSettings() {#constructor}

Initializes a new instance of the [`Bzip2CompressionSettings`](../) class with default block size, equals to 9 hundred of kilobytes.

```csharp
public Bzip2CompressionSettings()
```

## Examples

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### See Also

* class [Bzip2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)


