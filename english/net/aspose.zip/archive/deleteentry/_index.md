---
title: DeleteEntry
second_title: Aspose.ZIP for .NET API Reference
description: 
type: docs
weight: 60
url: /net/aspose.zip/archive/deleteentry/
---
## Archive.DeleteEntry method (1 of 2)

Removes the first occurrence of a specific entry from the entries list.

```csharp
public Archive DeleteEntry(ArchiveEntry entry)
```

| Parameter | Type | Description |
| --- | --- | --- |
| entry | ArchiveEntry | The entry to remove from the entries list. |

## Return Value

The archive with the entry deleted.

### Examples

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

* class [ArchiveEntry](../../archiveentry)
* class [Archive](../../archive)
* namespace [Aspose.Zip](../../archive)
* assembly [Aspose.Zip](../../../)

---

## Archive.DeleteEntry method (2 of 2)

Removes the entry from the entries list by index.

```csharp
public Archive DeleteEntry(int entryIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | Int32 | The zero-based index of the entry to remove. |

## Return Value

The archive with the entry deleted.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex* is less than 0.-or- *entryIndex* is equal to or greater than `Entries` count. |

### Examples

```csharp
using (var archive = new TarArchive("two_files.zip"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.zip");
}
```

### See Also

* class [Archive](../../archive)
* namespace [Aspose.Zip](../../archive)
* assembly [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.ZIP.dll -->