---
title: SharArchive.DeleteEntry
second_title: Aspose.ZIP för .NET API-referens
description: SharArchive metod. Tar bort den första förekomsten av en specifik post från postlistan.
type: docs
weight: 50
url: /sv/net/aspose.zip.shar/shararchive/deleteentry/
---
## DeleteEntry(SharEntry) {#deleteentry}

Tar bort den första förekomsten av en specifik post från postlistan.

```csharp
public SharArchive DeleteEntry(SharEntry entry)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| entry | SharEntry | Posten som ska tas bort från postlistan. |

### Returvärde

Shar-inträdesinstans.

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *entry* är inget. |

### Exempel

Så här kan du ta bort alla poster utom den sista:

```csharp
using (var archive = new SharArchive("archive.shar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputSharFile);
}
```

### Se även

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* namnutrymme [Aspose.Zip.Shar](../../shararchive/)
* hopsättning [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Tar bort posten från postlistan efter index.

```csharp
public SharArchive DeleteEntry(int entryIndex)
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
using (var archive = new SharArchive("two_files.shar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.shar");
}
```

### Se även

* class [SharArchive](../)
* namnutrymme [Aspose.Zip.Shar](../../shararchive/)
* hopsättning [Aspose.Zip](../../../)


