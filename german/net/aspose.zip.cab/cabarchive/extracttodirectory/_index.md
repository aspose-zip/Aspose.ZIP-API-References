---
title: CabArchive.ExtractToDirectory
second_title: Aspose.ZIP für .NET-API-Referenz
description: CabArchive methode. Extrahiert alle Dateien im Archiv in das angegebene Verzeichnis.
type: docs
weight: 40
url: /de/net/aspose.zip.cab/cabarchive/extracttodirectory/
---
## CabArchive.ExtractToDirectory method

Extrahiert alle Dateien im Archiv in das angegebene Verzeichnis.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationDirectory | String | Der Pfad zu dem Verzeichnis, in dem die extrahierten Dateien abgelegt werden sollen. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | Pfad ist null |
| PathTooLongException | Der angegebene Pfad, Dateiname oder beide überschreiten die vom System definierte maximale Länge. |
| SecurityException | Der Anrufer hat nicht die erforderliche Berechtigung, auf das vorhandene Verzeichnis zuzugreifen. |
| NotSupportedException | Wenn das Verzeichnis nicht vorhanden ist, enthält der Pfad einen Doppelpunkt (:), der nicht Teil einer Laufwerksbezeichnung ist ("C:\"). |
| ArgumentException | Pfad ist eine leere Zeichenfolge, enthält nur Leerzeichen oder enthält ein oder mehrere ungültige Zeichen. Sie können ungültige Zeichen mithilfe der System.IO.Path.GetInvalidPathChars-Methode abfragen. -oder- Pfad hat ein Präfix oder enthält nur einen Doppelpunkt (:). |
| IOException | Das durch Pfad angegebene Verzeichnis ist eine Datei. -oder- Der Netzwerkname ist nicht bekannt. |

### Bemerkungen

Wenn das Verzeichnis nicht existiert, wird es erstellt.

### Beispiele

```csharp
using (var archive = new CabArchive("archive.cab")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Siehe auch

* class [CabArchive](../)
* namensraum [Aspose.Zip.Cab](../../cabarchive/)
* Montage [Aspose.Zip](../../../)


