---
title: CpioArchive.DeleteEntry
second_title: Aspose.ZIP voor .NET API-referentie
description: CpioArchive methode. Verwijdert het eerste exemplaar van een specifiek item uit de lijst met items.
type: docs
weight: 50
url: /nl/net/aspose.zip.cpio/cpioarchive/deleteentry/
---
## DeleteEntry(CpioEntry) {#deleteentry}

Verwijdert het eerste exemplaar van een specifiek item uit de lijst met items.

```csharp
public CpioArchive DeleteEntry(CpioEntry entry)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| entry | CpioEntry | Het item dat uit de lijst met items moet worden verwijderd. |

### Winstwaarde

Cpio ingangsinstantie.

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *entry* is niets. |

### Voorbeelden

Hier ziet u hoe u alle vermeldingen behalve de laatste kunt verwijderen:

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputCpioFile);
}
```

### Zie ook

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* naamruimte [Aspose.Zip.Cpio](../../cpioarchive/)
* montage [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Verwijdert het item uit de lijst met items op index.

```csharp
public CpioArchive DeleteEntry(int entryIndex)
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
using (var archive = new CpioArchive("two_files.cpio"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.cpio");
}
```

### Zie ook

* class [CpioArchive](../)
* naamruimte [Aspose.Zip.Cpio](../../cpioarchive/)
* montage [Aspose.Zip](../../../)


