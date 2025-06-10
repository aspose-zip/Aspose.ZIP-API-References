---
title: CpioArchive.DeleteEntry
second_title: Aspose.ZIP for .NET API Reference
description: CpioArchive method. Removes the first occurrence of a specific entry from the entry list
type: docs
weight: 50
url: /net/aspose.zip.cpio/cpioarchive/deleteentry/
---
## DeleteEntry(CpioEntry) {#deleteentry}

Removes the first occurrence of a specific entry from the entry list.

```csharp
public CpioArchive DeleteEntry(CpioEntry entry)
```

| Parameter | Type | Description |
| --- | --- | --- |
| entry | CpioEntry | The entry to remove from the entries list. |

### Return Value

Cpio entry instance.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *entry* is null. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

## Examples

Here is how you can remove all entries except the last one:

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputCpioFile);
}
```

### See Also

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Removes the entry from the entry list by index.

```csharp
public CpioArchive DeleteEntry(int entryIndex)
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
using (var archive = new CpioArchive("two_files.cpio"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.cpio");
}
```

### See Also

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


