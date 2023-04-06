---
title: CpioArchive.DeleteEntry
second_title: Aspose.ZIP für .NET-API-Referenz
description: CpioArchive methode. Entfernt das erste Vorkommen eines bestimmten Eintrags aus der Eintragsliste.
type: docs
weight: 50
url: /de/net/aspose.zip.cpio/cpioarchive/deleteentry/
---
## DeleteEntry(CpioEntry) {#deleteentry}

Entfernt das erste Vorkommen eines bestimmten Eintrags aus der Eintragsliste.

```csharp
public CpioArchive DeleteEntry(CpioEntry entry)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| entry | CpioEntry | Der Eintrag, der aus der Eintragsliste entfernt werden soll. |

### Rückgabewert

Cpio-Eintragsinstanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *entry* ist Null. |

### Beispiele

So entfernen Sie alle Einträge bis auf den letzten:

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputCpioFile);
}
```

### Siehe auch

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* namensraum [Aspose.Zip.Cpio](../../cpioarchive/)
* Montage [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Entfernt den Eintrag aus der Eintragsliste nach Index.

```csharp
public CpioArchive DeleteEntry(int entryIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| entryIndex | Int32 | Der nullbasierte Index des zu entfernenden Eintrags. |

### Rückgabewert

Das Archiv mit dem gelöschten Eintrag.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex* ist kleiner als 0.-oder-*entryIndex* ist gleich oder größer als`Einträge` zählen. |

### Beispiele

```csharp
using (var archive = new CpioArchive("two_files.cpio"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.cpio");
}
```

### Siehe auch

* class [CpioArchive](../)
* namensraum [Aspose.Zip.Cpio](../../cpioarchive/)
* Montage [Aspose.Zip](../../../)


