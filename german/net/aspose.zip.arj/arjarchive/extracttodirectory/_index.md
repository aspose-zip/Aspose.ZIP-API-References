---
title: "ArjArchive.ExtractToDirectory"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "ArjArchive‑Methode. Extrahiert alle Einträge in das angegebene Verzeichnis"
type: docs
weight: 60
url: /de/net/aspose.zip.arj/arjarchive/extracttodirectory/
---
## ArjArchive.ExtractToDirectory method

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
| ArgumentNullException | Wird ausgelöst, wenn das *destinationDirectory* null ist. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| OperationCanceledException | In .NET Framework 4.0 und höher: Wird ausgelöst, wenn die Extraktion über das bereitgestellte Abbruch-Token abgebrochen wird. |
| InvalidDataException | Prüfsummen‑Fehler für Header oder Daten. – oder – Das Archiv ist beschädigt. |
| NotImplementedException | Eintrag komprimiert mit Methode 4. |

## Beispiele

Das folgende Beispiel zeigt, wie alle Einträge in ein Verzeichnis extrahiert werden:

```csharp
using (var archive = new ArjArchive(File.OpenRead("archive.arj")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Siehe auch

* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


