---
title: Archive.DeleteEntry
second_title: Aspose.ZIP voor .NET API-referentie
description: Archive methode. Verwijdert het eerste exemplaar van een specifiek item uit de lijst met items.
type: docs
weight: 60
url: /nl/net/aspose.zip/archive/deleteentry/
---
## DeleteEntry(ArchiveEntry) {#deleteentry}

Verwijdert het eerste exemplaar van een specifiek item uit de lijst met items.

```csharp
public Archive DeleteEntry(ArchiveEntry entry)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| entry | ArchiveEntry | Het item dat uit de lijst met items moet worden verwijderd. |

### Winstwaarde

Het archief met het verwijderde item.

### Voorbeelden

Hier ziet u hoe u alle vermeldingen behalve de laatste kunt verwijderen:

```csharp
using (var archive = new Archive("archive.zip"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save("last_entry.zip");
}
```

### Zie ook

* class [ArchiveEntry](../../archiveentry/)
* class [Archive](../)
* naamruimte [Aspose.Zip](../../archive/)
* montage [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Verwijdert het item uit de lijst met items op index.

```csharp
public Archive DeleteEntry(int entryIndex)
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
using (var archive = new TarArchive("two_files.zip"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.zip");
}
```

### Zie ook

* class [Archive](../)
* naamruimte [Aspose.Zip](../../archive/)
* montage [Aspose.Zip](../../../)


