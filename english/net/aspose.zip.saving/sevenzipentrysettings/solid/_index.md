---
title: SevenZipEntrySettings.Solid
second_title: Aspose.ZIP for .NET API Reference
description: SevenZipEntrySettings property. Gets or sets value indicating whether to concatenate entries and treat them as a single data block
type: docs
weight: 50
url: /net/aspose.zip.saving/sevenzipentrysettings/solid/
---
## SevenZipEntrySettings.Solid property

Gets or sets value indicating whether to concatenate entries and treat them as a single data block.

```csharp
public bool Solid { get; set; }
```

## Remarks

Provide `SevenZipEntrySettings` for solid 7z archive on archive instantiation.

## Examples

The following example shows how to compress a directory to solid 7z archive with LZMA2 compression without encryption.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings()){ Solid = true }))
    {
        archive.CreateEntries("C:\\Documents");
        archive.Save(sevenZipFile);
    }
}
```

### See Also

* class [SevenZipEntrySettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipentrysettings/)
* assembly [Aspose.Zip](../../../)


