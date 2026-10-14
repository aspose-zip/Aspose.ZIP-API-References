---
title: "IsoArchive.CreateDirectory"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "IsoArchive-Methode. Fügt dem ISO-Image ein Verzeichnis hinzu"
type: docs
weight: 30
url: /de/net/aspose.zip.iso/isoarchive/createdirectory/
---
## IsoArchive.CreateDirectory method

Fügt dem ISO-Image ein Verzeichnis hinzu.

```csharp
public IsoEntry CreateDirectory(string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Pfad des Verzeichnisses im ISO. |

### Rückgabewert

Der ISO-Eintrag wurde erstellt.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| InvalidOperationException | Das Archiv ist zum Extrahieren geöffnet. |
| ArgumentNullException | `name` ist null oder leer. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

### Siehe auch

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


