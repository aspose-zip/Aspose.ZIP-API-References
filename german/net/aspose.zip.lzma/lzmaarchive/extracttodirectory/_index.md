---
title: "LzmaArchive.ExtractToDirectory"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "LzmaArchive Methode. Extrahiert den Inhalt des Archivs in das angegebene Verzeichnis."
type: docs
weight: 40
url: /de/net/aspose.zip.lzma/lzmaarchive/extracttodirectory/
---
## LzmaArchive.ExtractToDirectory method

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
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| ArgumentNullException | *destinationDirectory* ist null. |
| PathTooLongException | Der angegebene Pfad, Dateiname oder beides überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen kürzer als 248 Zeichen sein und Dateinamen kürzer als 260 Zeichen. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung, auf das vorhandene Verzeichnis zuzugreifen. |
| NotSupportedException | Wenn das Verzeichnis nicht existiert, enthält der Pfad ein Doppelpunktzeichen (:) das nicht Teil einer Laufwerksbezeichnung (\"C:\\") ist. |
| ArgumentException | *destinationDirectory* ist ein leerer String, enthält nur Leerzeichen oder enthält ein oder mehrere ungültige Zeichen. Sie können nach ungültigen Zeichen fragen, indem Sie die Methode System.IO.Path.GetInvalidPathChars verwenden. -or- Pfad ist mit nur einem Doppelpunktzeichen (:) vorangestellt oder enthält nur einen Doppelpunkt. |
| IOException | Das durch den Pfad angegebene Verzeichnis ist eine Datei. -or- Der Netzwerkname ist nicht bekannt. |
| InvalidDataException | Das Archiv ist beschädigt. |

## Hinweise

Wenn das Verzeichnis nicht existiert, wird es erstellt.

### Siehe auch

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)


