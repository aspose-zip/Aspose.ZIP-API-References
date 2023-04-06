---
title: XarDirectoryEntry.ExtractToDirectory
second_title: Aspose.ZIP für .NET-API-Referenz
description: XarDirectoryEntry methode. Extrahiert alle Dateien im aktuellen Verzeichnis in das angegebene Verzeichnis.
type: docs
weight: 50
url: /de/net/aspose.zip.xar/xardirectoryentry/extracttodirectory/
---
## XarDirectoryEntry.ExtractToDirectory method

Extrahiert alle Dateien im aktuellen Verzeichnis in das angegebene Verzeichnis.

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
| PathTooLongException | Der angegebene Pfad, Dateiname oder beide überschreiten die vom System definierte maximale Länge. Beispielsweise müssen auf Windows-basierten Plattformen Pfade weniger als 248 Zeichen und Dateinamen weniger als 260 Zeichen umfassen. |
| SecurityException | Der Anrufer hat nicht die erforderliche Berechtigung, auf das vorhandene Verzeichnis zuzugreifen. |
| NotSupportedException | Wenn das Verzeichnis nicht vorhanden ist, enthält der Pfad einen Doppelpunkt (:), der nicht Teil einer Laufwerksbezeichnung ist ("C:\"). |
| ArgumentException | Pfad ist eine leere Zeichenfolge, enthält nur Leerzeichen oder enthält ein oder mehrere ungültige Zeichen. Sie können ungültige Zeichen mithilfe der System.IO.Path.GetInvalidPathChars-Methode abfragen. -oder- Pfad hat ein Präfix oder enthält nur einen Doppelpunkt (:). |
| IOException | Das durch Pfad angegebene Verzeichnis ist eine Datei. -oder- Der Netzwerkname ist nicht bekannt. |

### Bemerkungen

Wenn das Verzeichnis nicht existiert, wird es erstellt.

### Beispiele

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   archive.Directories.First().ExtractToDirectory("C:\\extracted");
}
```

### Siehe auch

* class [XarDirectoryEntry](../)
* namensraum [Aspose.Zip.Xar](../../xardirectoryentry/)
* Montage [Aspose.Zip](../../../)


