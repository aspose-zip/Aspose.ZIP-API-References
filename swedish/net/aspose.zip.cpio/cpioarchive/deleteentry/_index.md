---
title: CpioArchive.DeleteEntry
second_title: Aspose.ZIP för .NET API-referens
description: CpioArchive metod. Tar bort den första förekomsten av en specifik post från postlistan.
type: docs
weight: 50
url: /sv/net/aspose.zip.cpio/cpioarchive/deleteentry/
---
## DeleteEntry(CpioEntry) {#deleteentry}

Tar bort den första förekomsten av en specifik post från postlistan.

```csharp
public CpioArchive DeleteEntry(CpioEntry entry)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| entry | CpioEntry | Posten som ska tas bort från postlistan. |

### Returvärde

Cpio-inmatningsinstans.

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *entry* är inget. |

### Exempel

Så här kan du ta bort alla poster utom den sista:

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputCpioFile);
}
```

### Se även

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* namnutrymme [Aspose.Zip.Cpio](../../cpioarchive/)
* hopsättning [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Tar bort posten från postlistan efter index.

```csharp
public CpioArchive DeleteEntry(int entryIndex)
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
using (var archive = new CpioArchive("two_files.cpio"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.cpio");
}
```

### Se även

* class [CpioArchive](../)
* namnutrymme [Aspose.Zip.Cpio](../../cpioarchive/)
* hopsättning [Aspose.Zip](../../../)


