---
title: TarArchive.DeleteEntry
second_title: Aspose.ZIP for .NET API Reference
description: TarArchive method. Removes the first occurrence of a specific entry from the entry list
type: docs
weight: 120
url: /net/aspose.zip.tar/tararchive/deleteentry/
---
## DeleteEntry(TarEntry) {#deleteentry}

Removes the first occurrence of a specific entry from the entry list.

```csharp
public TarArchive DeleteEntry(TarEntry entry)
```

| Parameter | Type | Description |
| --- | --- | --- |
| entry | TarEntry | The entry to remove from the entries list. |

### Return Value

The archive with the entry deleted.

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | Archive has been disposed and cannot be used |

## Examples

Here is how you can remove all entries except the last one:

```csharp
using (var archive = new TarArchive("archive.tar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputTarFile);
}
```

### See Also

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Removes the entry from the entry list by index.

```csharp
public TarArchive DeleteEntry(int entryIndex)
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
| ObjectDisposedException | Archive has been disposed and cannot be used |

## Examples

```csharp
using (var archive = new TarArchive("two_files.tar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.tar");
}
```

### See Also

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


