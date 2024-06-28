---
title: SevenZipPPMdCompressionSettings.SevenZipPPMdCompressionSettings
second_title: Aspose.ZIP for .NET API Reference
description: SevenZipPPMdCompressionSettings constructor. Instantiates settings for PPMd compression method within 7z archive
type: docs
weight: 10
url: /net/aspose.zip.saving/sevenzipppmdcompressionsettings/sevenzipppmdcompressionsettings/
---
## SevenZipPPMdCompressionSettings(byte, int) {#constructor_1}

Instantiates settings for PPMd compression method within 7z archive.

```csharp
public SevenZipPPMdCompressionSettings(byte maxOrder, int suballocatorSize)
```

| Parameter | Type | Description |
| --- | --- | --- |
| maxOrder | Byte | Maximum order. |
| suballocatorSize | Int32 | Memory size in MB suballocator may consume. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | *maxOrder* is not between 2 and 32, or *suballocatorSize* is not between 1 and 1024. |

## Remarks

Bigger model orders almost surely results in better compression and surely more memory and CPU usage.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse.

## Examples

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32))))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### See Also

* class [SevenZipPPMdCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipPPMdCompressionSettings() {#constructor}

Instantiates settings for PPMd compression method within 7z archive with default model order and sub-allocator size.

```csharp
public SevenZipPPMdCompressionSettings()
```

## Remarks

Default model order is 6 and sub-allocator size is 16MB.

## Examples

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### See Also

* class [SevenZipPPMdCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* assembly [Aspose.Zip](../../../)


