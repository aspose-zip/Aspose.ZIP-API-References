---
title: SharArchive.DeleteEntry
second_title: Aspose.ZIP for .NET API Reference
description: SharArchive method. Removes the first occurrence of a specific entry from the entry list
type: docs
weight: 50
url: /net/aspose.zip.shar/shararchive/deleteentry/
---
## DeleteEntry(SharEntry) {#deleteentry}

Removes the first occurrence of a specific entry from the entry list.

```csharp
public SharArchive DeleteEntry(SharEntry entry)
```

| Parameter | Type | Description |
| --- | --- | --- |
| entry | SharEntry | The entry to remove from the entries list. |

### Return Value

Shar entry instance.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *entry* is null. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

## Examples

Here is how you can remove all entries except the last one:

```csharp
using (var archive = new SharArchive("archive.shar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputSharFile);
}
```

### See Also

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Removes the entry from the entry list by index.

```csharp
public SharArchive DeleteEntry(int entryIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | Int32 | The zero-based index of the entry to remove. |

### Return Value

The archive with the entry deleted.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex* is less than 0.-or- *entryIndex* is equal to or greater than `Entries` count. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

## Examples

```csharp
using (var archive = new SharArchive("two_files.shar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.shar");
}
```

### See Also

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


