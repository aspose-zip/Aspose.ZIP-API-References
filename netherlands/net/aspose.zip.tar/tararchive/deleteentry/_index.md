---
title: TarArchive.DeleteEntry
second_title: Aspose.ZIP voor .NET API-referentie
description: TarArchive methode. Verwijdert het eerste exemplaar van een specifiek item uit de lijst met items.
type: docs
weight: 90
url: /nl/net/aspose.zip.tar/tararchive/deleteentry/
---
## DeleteEntry(TarEntry) {#deleteentry}

Verwijdert het eerste exemplaar van een specifiek item uit de lijst met items.

```csharp
public TarArchive DeleteEntry(TarEntry entry)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| entry | TarEntry | Het item dat uit de lijst met items moet worden verwijderd. |

### Winstwaarde

Het archief met het verwijderde item.

### Voorbeelden

Hier ziet u hoe u alle vermeldingen behalve de laatste kunt verwijderen:

```csharp
using (var archive = new TarArchive("archive.tar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputTarFile);
}
```

### Zie ook

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* naamruimte [Aspose.Zip.Tar](../../tararchive/)
* montage [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Verwijdert het item uit de lijst met items op index.

```csharp
public TarArchive DeleteEntry(int entryIndex)
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
using (var archive = new TarArchive("two_files.tar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.tar");
}
```

### Zie ook

* class [TarArchive](../)
* naamruimte [Aspose.Zip.Tar](../../tararchive/)
* montage [Aspose.Zip](../../../)


