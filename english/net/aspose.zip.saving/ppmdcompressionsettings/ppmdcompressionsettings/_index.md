---
title: PPMdCompressionSettings.PPMdCompressionSettings
second_title: Aspose.ZIP for .NET API Reference
description: PPMdCompressionSettings constructor. Initializes a new instance of the PPMdCompressionSettings class
type: docs
weight: 10
url: /net/aspose.zip.saving/ppmdcompressionsettings/ppmdcompressionsettings/
---
## PPMdCompressionSettings(int, int) {#constructor_1}

Initializes a new instance of the [`PPMdCompressionSettings`](../) class.

```csharp
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```

| Parameter | Type | Description |
| --- | --- | --- |
| modelOrder | Int32 | Order of the model. |
| suballocatorSize | Int32 | Memory size in MB suballocator may consume. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | *modelOrder* is not between 2 and 16. - or - *suballocatorSize* is not between 1 and 256. |

## Remarks

Bigger model orders almost surely results in better compression and surely more memory and CPU usage.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse.

## Examples

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10))))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### See Also

* class [PPMdCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## PPMdCompressionSettings() {#constructor}

Initializes a new instance of the [`PPMdCompressionSettings`](../) class with default model order and sub-allocator size.

```csharp
public PPMdCompressionSettings()
```

## Remarks

The default model order is 8, and the sub-allocator size is 50MB.

## Examples

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### See Also

* class [PPMdCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* assembly [Aspose.Zip](../../../)


