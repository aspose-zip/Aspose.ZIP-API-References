---
title: XarArchive.DeleteEntry
second_title: Aspose.ZIP for .NET API Reference
description: XarArchive method. Removes the first occurrence of a specific entry from the entry list
type: docs
weight: 50
url: /net/aspose.zip.xar/xararchive/deleteentry/
---
## XarArchive.DeleteEntry method

Removes the first occurrence of a specific entry from the entry list.

```csharp
public XarArchive DeleteEntry(XarEntry entry)
```

| Parameter | Type | Description |
| --- | --- | --- |
| entry | XarEntry | The entry to remove from the entries list. |

### Return Value

Xar entry instance.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *entry* is null. |

## Examples

Here is how you can remove all entries except the last one:

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries.FirstOrDefault());
    archive.Save(outputXarFile);
}
```

### See Also

* class [XarEntry](../../xarentry/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


