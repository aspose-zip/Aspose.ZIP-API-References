---
title: "XarArchive.DeleteEntry"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "XarArchive-Methode. Entfernt das erste Vorkommen eines bestimmten Eintrags aus der Eintragsliste"
type: docs
weight: 50
url: /de/net/aspose.zip.xar/xararchive/deleteentry/
---
## XarArchive.DeleteEntry method

Entfernt das erste Vorkommen eines bestimmten Eintrags aus der Eintragsliste.

```csharp
public XarArchive DeleteEntry(XarEntry entry)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Eintrag | XarEntry | Der Eintrag, der aus der Eintragsliste entfernt werden soll. |

### Rückgabewert

Xar-Eintrag-Instanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *entry* ist null. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| InvalidOperationException | Das Archiv ist nicht zum Extrahieren geöffnet. |

## Beispiele

So können Sie alle Einträge außer dem letzten entfernen:

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries.FirstOrDefault());
    archive.Save(outputXarFile);
}
```

### Siehe auch

* class [XarEntry](../../xarentry/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


