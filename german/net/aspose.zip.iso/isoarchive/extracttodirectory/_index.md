---
title: "IsoArchive.ExtractToDirectory"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "IsoArchive-Methode. Extrahiert alle Einträge in das angegebene Verzeichnis"
type: docs
weight: 60
url: /de/net/aspose.zip.iso/isoarchive/extracttodirectory/
---
## IsoArchive.ExtractToDirectory method

Extrahiert alle Einträge in das angegebene Verzeichnis.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationDirectory | String | Das Verzeichnis, in das die Einträge extrahiert werden. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| InvalidOperationException | Wird ausgelöst, wenn das Archiv im Bearbeitungsmodus ist. |
| ArgumentNullException | Wird ausgelöst, wenn das *destinationDirectory* null ist. |
| OperationCanceledException | In .NET Framework 4.0 und höher: Wird ausgelöst, wenn die Extraktion über das bereitgestellte Abbruch-Token abgebrochen wird. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

## Beispiele

Das folgende Beispiel zeigt, wie alle Einträge in ein Verzeichnis extrahiert werden:

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Siehe auch

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


