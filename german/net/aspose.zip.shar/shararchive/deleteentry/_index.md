---
title: SharArchive.DeleteEntry
second_title: Aspose.ZIP für .NET-API-Referenz
description: SharArchive methode. Entfernt das erste Vorkommen eines bestimmten Eintrags aus der Eintragsliste.
type: docs
weight: 50
url: /de/net/aspose.zip.shar/shararchive/deleteentry/
---
## DeleteEntry(SharEntry) {#deleteentry}

Entfernt das erste Vorkommen eines bestimmten Eintrags aus der Eintragsliste.

```csharp
public SharArchive DeleteEntry(SharEntry entry)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| entry | SharEntry | Der Eintrag, der aus der Eintragsliste entfernt werden soll. |

### Rückgabewert

Instanz des Shar-Eintrags.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *entry* ist Null. |

### Beispiele

So entfernen Sie alle Einträge bis auf den letzten:

```csharp
using (var archive = new SharArchive("archive.shar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputSharFile);
}
```

### Siehe auch

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* namensraum [Aspose.Zip.Shar](../../shararchive/)
* Montage [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Entfernt den Eintrag aus der Eintragsliste nach Index.

```csharp
public SharArchive DeleteEntry(int entryIndex)
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
using (var archive = new SharArchive("two_files.shar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.shar");
}
```

### Siehe auch

* class [SharArchive](../)
* namensraum [Aspose.Zip.Shar](../../shararchive/)
* Montage [Aspose.Zip](../../../)


