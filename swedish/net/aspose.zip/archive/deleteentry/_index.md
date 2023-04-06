---
title: Archive.DeleteEntry
second_title: Aspose.ZIP för .NET API-referens
description: Archive metod. Tar bort den första förekomsten av en specifik post från postlistan.
type: docs
weight: 60
url: /sv/net/aspose.zip/archive/deleteentry/
---
## DeleteEntry(ArchiveEntry) {#deleteentry}

Tar bort den första förekomsten av en specifik post från postlistan.

```csharp
public Archive DeleteEntry(ArchiveEntry entry)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| entry | ArchiveEntry | Posten som ska tas bort från postlistan. |

### Returvärde

Arkivet med posten raderad.

### Exempel

Så här kan du ta bort alla poster utom den sista:

```csharp
using (var archive = new Archive("archive.zip"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save("last_entry.zip");
}
```

### Se även

* class [ArchiveEntry](../../archiveentry/)
* class [Archive](../)
* namnutrymme [Aspose.Zip](../../archive/)
* hopsättning [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Tar bort posten från postlistan efter index.

```csharp
public Archive DeleteEntry(int entryIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| entryIndex | Int32 | Det nollbaserade indexet för posten som ska tas bort. |

### Returvärde

Arkivet med posten raderad.

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex* är mindre än 0.-eller-*entryIndex* är lika med eller större än`Inlägg` räkna. |

### Exempel

```csharp
using (var archive = new TarArchive("two_files.zip"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.zip");
}
```

### Se även

* class [Archive](../)
* namnutrymme [Aspose.Zip](../../archive/)
* hopsättning [Aspose.Zip](../../../)


