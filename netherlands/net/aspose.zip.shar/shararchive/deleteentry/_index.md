---
title: SharArchive.DeleteEntry
second_title: Aspose.ZIP voor .NET API-referentie
description: SharArchive methode. Verwijdert het eerste exemplaar van een specifiek item uit de lijst met items.
type: docs
weight: 50
url: /nl/net/aspose.zip.shar/shararchive/deleteentry/
---
## DeleteEntry(SharEntry) {#deleteentry}

Verwijdert het eerste exemplaar van een specifiek item uit de lijst met items.

```csharp
public SharArchive DeleteEntry(SharEntry entry)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| entry | SharEntry | Het item dat uit de lijst met items moet worden verwijderd. |

### Winstwaarde

Shar entry-exemplaar.

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *entry* is niets. |

### Voorbeelden

Hier ziet u hoe u alle vermeldingen behalve de laatste kunt verwijderen:

```csharp
using (var archive = new SharArchive("archive.shar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputSharFile);
}
```

### Zie ook

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* naamruimte [Aspose.Zip.Shar](../../shararchive/)
* montage [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Verwijdert het item uit de lijst met items op index.

```csharp
public SharArchive DeleteEntry(int entryIndex)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| entryIndex | Int32 | De op nul gebaseerde index van het item dat moet worden verwijderd. |

### Winstwaarde

Het archief met het verwijderde item.

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex* is kleiner dan 0.-of-*entryIndex* is gelijk aan of groter dan`Inzendingen` graaf. |

### Voorbeelden

```csharp
using (var archive = new SharArchive("two_files.shar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.shar");
}
```

### Zie ook

* class [SharArchive](../)
* naamruimte [Aspose.Zip.Shar](../../shararchive/)
* montage [Aspose.Zip](../../../)


