---
title: TarArchive.DeleteEntry
second_title: Aspose.ZIP för .NET API-referens
description: TarArchive metod. Tar bort den första förekomsten av en specifik post från postlistan.
type: docs
weight: 90
url: /sv/net/aspose.zip.tar/tararchive/deleteentry/
---
## DeleteEntry(TarEntry) {#deleteentry}

Tar bort den första förekomsten av en specifik post från postlistan.

```csharp
public TarArchive DeleteEntry(TarEntry entry)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| entry | TarEntry | Posten som ska tas bort från postlistan. |

### Returvärde

Arkivet med posten raderad.

### Exempel

Så här kan du ta bort alla poster utom den sista:

```csharp
using (var archive = new TarArchive("archive.tar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputTarFile);
}
```

### Se även

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* namnutrymme [Aspose.Zip.Tar](../../tararchive/)
* hopsättning [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Tar bort posten från postlistan efter index.

```csharp
public TarArchive DeleteEntry(int entryIndex)
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
using (var archive = new TarArchive("two_files.tar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.tar");
}
```

### Se även

* class [TarArchive](../)
* namnutrymme [Aspose.Zip.Tar](../../tararchive/)
* hopsättning [Aspose.Zip](../../../)


