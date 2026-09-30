---
title: "Lz4Archive.ExtractToDirectory"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "Lz4Archive-Methode. Extrahiert den Inhalt des Archivs in das angegebene Verzeichnis"
type: docs
weight: 40
url: /de/net/aspose.zip.lz4/lz4archive/extracttodirectory/
---
## Lz4Archive.ExtractToDirectory method

Extrahiert den Inhalt des Archivs in das bereitgestellte Verzeichnis.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationDirectory | String | Der Pfad zum Verzeichnis, in dem die extrahierten Dateien abgelegt werden sollen. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *destinationDirectory* ist null. |
| PathTooLongException | Der angegebene Pfad, Dateiname oder beides überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen kürzer als 248 Zeichen sein und Dateinamen kürzer als 260 Zeichen. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung, auf das vorhandene Verzeichnis zuzugreifen. |
| NotSupportedException | Wenn das Verzeichnis nicht existiert, enthält der Pfad ein Doppelpunktzeichen (:) das nicht Teil einer Laufwerksbezeichnung (\"C:\\") ist. |
| ArgumentException | *destinationDirectory* ist ein leerer String, enthält nur Leerzeichen oder enthält ein oder mehrere ungültige Zeichen. Sie können nach ungültigen Zeichen fragen, indem Sie die Methode System.IO.Path.GetInvalidPathChars verwenden. -or- Pfad ist mit nur einem Doppelpunktzeichen (:) vorangestellt oder enthält nur einen Doppelpunkt. |
| IOException | Das durch den Pfad angegebene Verzeichnis ist eine Datei. -or- Der Netzwerkname ist nicht bekannt. |
| EndOfStreamException | Quellstream ist zu kurz. |
| InvalidDataException | Falsche Bytes gefunden beim Initialisieren der Dekodierung. |
| InvalidOperationException | Das Archiv ist für die Zusammensetzung vorbereitet. |
| OperationCanceledException | In .NET Framework 4.0 und höher: Wird ausgelöst, wenn die Extraktion über das bereitgestellte Abbruch-Token abgebrochen wird. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

## Hinweise

Wenn das Verzeichnis nicht existiert, wird es erstellt.

### Siehe auch

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


