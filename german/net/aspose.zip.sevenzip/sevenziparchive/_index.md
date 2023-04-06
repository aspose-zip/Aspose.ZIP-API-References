---
title: Class SevenZipArchive
second_title: Aspose.ZIP für .NET-API-Referenz
description: Aspose.Zip.SevenZip.SevenZipArchive klas. Diese Klasse repräsentiert eine 7zArchivdatei. Verwenden Sie es zum Erstellen und Extrahieren von 7zArchiven.
type: docs
weight: 660
url: /de/net/aspose.zip.sevenzip/sevenziparchive/
---
## SevenZipArchive class

Diese Klasse repräsentiert eine 7z-Archivdatei. Verwenden Sie es zum Erstellen und Extrahieren von 7z-Archiven.

```csharp
public class SevenZipArchive : IArchive
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [SevenZipArchive](sevenziparchive/#constructor)(SevenZipEntrySettings) | Initialisiert eine neue Instanz von`SevenZipArchive` Klasse mit optionalen Einstellungen für ihre Einträge. |
| [SevenZipArchive](sevenziparchive/#constructor_1)(Stream) | Initialisiert eine neue Instanz von`SevenZipArchive` Klasse und Liste der zusammengesetzten Einträge können aus dem Archiv extrahiert werden. |
| [SevenZipArchive](sevenziparchive/#constructor_2)(string) | Initialisiert eine neue Instanz von`SevenZipArchive` Klasse und Liste der zusammengesetzten Einträge können aus dem Archiv extrahiert werden. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Entries](../../aspose.zip.sevenzip/sevenziparchive/entries/) { get; } | Ruft Einträge von ab[`SevenZipArchiveEntry`](../sevenziparchiveentry/) Typ, der das Archiv bildet. |
| [NewEntrySettings](../../aspose.zip.sevenzip/sevenziparchive/newentrysettings/) { get; } | Komprimierungs- und Verschlüsselungseinstellungen, die für neu hinzugefügte verwendet werden[`SevenZipArchiveEntry`](../sevenziparchiveentry/) Artikel. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries)(DirectoryInfo, bool) | Fügt dem Archiv rekursiv alle Dateien und Verzeichnisse im angegebenen Verzeichnis hinzu. |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries_1)(string, bool) | Fügt dem Archiv rekursiv alle Dateien und Verzeichnisse im angegebenen Verzeichnis hinzu. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_1)(string, Stream, SevenZipEntrySettings) | Einzelner Eintrag im Archiv erstellen. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry)(string, FileInfo, bool, SevenZipEntrySettings) | Einzelner Eintrag im Archiv erstellen. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_2)(string, Stream, SevenZipEntrySettings, FileSystemInfo) | Einzelner Eintrag im Archiv erstellen. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_3)(string, string, bool, SevenZipEntrySettings) | Einzelner Eintrag im Archiv erstellen. |
| [Dispose](../../aspose.zip.sevenzip/sevenziparchive/dispose/)() | Führt anwendungsdefinierte Aufgaben aus, die mit dem Freigeben, Freigeben oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [ExtractToDirectory](../../aspose.zip.sevenzip/sevenziparchive/extracttodirectory/)(string, string) | Extrahiert alle Dateien im Archiv in das angegebene Verzeichnis. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save)(Stream) | Speichert das 7z-Archiv im bereitgestellten Stream. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save_1)(string) | Speichert das Archiv in der bereitgestellten Zieldatei. |
| [SaveSplit](../../aspose.zip.sevenzip/sevenziparchive/savesplit/)(string, SplitSevenZipArchiveSaveOptions) | Speichert mehrvolumiges Archiv im angegebenen Zielverzeichnis. |

### Siehe auch

* interface [IArchive](../../aspose.zip/iarchive/)
* namensraum [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* Montage [Aspose.Zip](../../)


