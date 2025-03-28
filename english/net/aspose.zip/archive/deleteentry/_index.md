---
title: Archive.DeleteEntry
second_title: Aspose.ZIP for .NET API Reference
description: Archive method. Removes the first occurrence of the specific entry from the entry list
type: docs
weight: 60
url: /net/aspose.zip/archive/deleteentry/
---
## DeleteEntry(ArchiveEntry) {#deleteentry}

Removes the first occurrence of the specific entry from the entry list.

```csharp
public Archive DeleteEntry(ArchiveEntry entry)
```

| Parameter | Type | Description |
| --- | --- | --- |
| entry | ArchiveEntry | The entry to remove from the entries list. |

### Return Value

The archive with the entry deleted.

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | The archive is disposed. |

## Examples

Here is how you can remove all entries except the last one:

```csharp
using (var archive = new Archive("archive.zip"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save("last_entry.zip");
}
```

### See Also

* class [ArchiveEntry](../../archiveentry/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Removes the entry from the entry list by index.

```csharp
public Archive DeleteEntry(int entryIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | Int32 | The zero-based index of the entry to remove. |

### Return Value

The archive with the entry deleted.

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | Archive is disposed. |
| ArgumentOutOfRangeException | *entryIndex* is less than 0.-or- *entryIndex* is equal to or greater than `Entries` count. |

## Examples

```csharp
using (var archive = new TarArchive("two_files.zip"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.zip");
}
```

### See Also

* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


