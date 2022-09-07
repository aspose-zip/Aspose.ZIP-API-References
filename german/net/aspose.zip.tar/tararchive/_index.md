---
title: TarArchive
second_title: Aspose.ZIP für .NET-API-Referenz
description: Diese Klasse repräsentiert eine tarArchivdatei. Verwenden Sie es um TarArchive zu erstellen zu extrahieren oder zu aktualisieren.
type: docs
weight: 600
url: /de/net/aspose.zip.tar/tararchive/
---
## TarArchive class

Diese Klasse repräsentiert eine tar-Archivdatei. Verwenden Sie es, um Tar-Archive zu erstellen, zu extrahieren oder zu aktualisieren.

```csharp
public class TarArchive : IDisposable
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [TarArchive](tararchive#constructor)() | Initialisiert eine neue Instanz von[`TarArchive`](../tararchive) Klasse. |
| [TarArchive](tararchive#constructor_1)(Stream) | Initialisiert eine neue Instanz von[`Archive`](../../aspose.zip/archive) Klasse und Liste der zusammengesetzten Einträge können aus dem Archiv extrahiert werden. |
| [TarArchive](tararchive#constructor_2)(string) | Initialisiert eine neue Instanz von[`TarArchive`](../tararchive) Klasse und Liste der zusammengesetzten Einträge können aus dem Archiv extrahiert werden. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Entries](../../aspose.zip.tar/tararchive/entries) { get; } | Ruft Einträge von ab[`TarEntry`](../tarentry) Typ, der das Archiv bildet. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip#fromgzip)(Stream) | Entpackt mitgeliefertes gzip-Archiv und setzt es zusammen[`TarArchive`](../tararchive) aus extrahierten Daten. |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip#fromgzip_1)(string) | Entpackt mitgeliefertes gzip-Archiv und setzt es zusammen[`TarArchive`](../tararchive) aus extrahierten Daten. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip#fromlzip)(Stream) | Extrahiert das mitgelieferte lzip-Archiv und setzt es zusammen[`TarArchive`](../tararchive) aus extrahierten Daten. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip#fromlzip_1)(string) | Extrahiert das mitgelieferte lzip-Archiv und setzt es zusammen[`TarArchive`](../tararchive) aus extrahierten Daten. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz#fromxz)(Stream) | Extrahiert das bereitgestellte Archiv im xz-Format und setzt es zusammen[`TarArchive`](../tararchive) aus extrahierten Daten. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz#fromxz_1)(string) | Extrahiert das bereitgestellte Archiv im xz-Format und setzt es zusammen[`TarArchive`](../tararchive) aus extrahierten Daten. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz#fromz)(Stream) | Extrahiert das bereitgestellte Archiv im Z-Format und setzt es zusammen[`TarArchive`](../tararchive) aus extrahierten Daten. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz#fromz_1)(string) | Extrahiert das bereitgestellte Archiv im Z-Format und setzt es zusammen[`TarArchive`](../tararchive) aus extrahierten Daten. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries#createentries)(DirectoryInfo, bool) | Fügt dem Archiv rekursiv alle Dateien und Verzeichnisse im angegebenen Verzeichnis hinzu. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries#createentries_1)(string, bool) | Fügt dem Archiv rekursiv alle Dateien und Verzeichnisse im angegebenen Verzeichnis hinzu. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry#createentry)(string, FileInfo, bool) | Einzelner Eintrag im Archiv erstellen. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry#createentry_1)(string, Stream, FileSystemInfo) | Einzelner Eintrag im Archiv erstellen. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry#createentry_2)(string, string, bool) | Einzelner Eintrag im Archiv erstellen. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry#deleteentry_1)(int) | Entfernt den Eintrag aus der Eintragsliste nach Index. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry#deleteentry)(TarEntry) | Entfernt das erste Vorkommen eines bestimmten Eintrags aus der Eintragsliste. |
| [Dispose](../../aspose.zip.tar/tararchive/dispose)() | Führt anwendungsdefinierte Aufgaben aus, die mit dem Freigeben, Freigeben oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [ExtractToDirectory](../../aspose.zip.tar/tararchive/extracttodirectory)(string) | Extrahiert alle Dateien im Archiv in das angegebene Verzeichnis. |
| [Save](../../aspose.zip.tar/tararchive/save#save)(Stream, TarFormat?) | Speichert das Archiv im bereitgestellten Stream. |
| [Save](../../aspose.zip.tar/tararchive/save#save_1)(string, TarFormat?) | Speichert das Archiv in der bereitgestellten Zieldatei. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped#savegzipped)(Stream, TarFormat?) | Speichert das Archiv mit gzip-Komprimierung im Stream. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped#savegzipped_1)(string, TarFormat?) | Speichert das Archiv in der Datei nach Pfad mit gzip-Komprimierung. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped#savelzipped)(Stream, TarFormat?) | Speichert das Archiv mit lzip-Komprimierung im Stream. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped#savelzipped_1)(string, TarFormat?) | Speichert das Archiv in der Datei nach Pfad mit lzip-Komprimierung. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed#savexzcompressed)(Stream, TarFormat?, XzArchiveSettings) | Speichert das Archiv mit xz-Komprimierung im Stream. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed#savexzcompressed_1)(string, TarFormat?, XzArchiveSettings) | Speichert das Archiv Pfad für Pfad mit xz-Komprimierung. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed#savezcompressed)(Stream, TarFormat?) | Speichert das Archiv mit Z-Komprimierung im Stream. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed#savezcompressed_1)(string, TarFormat?) | Speichert das Archiv Pfad für Pfad mit Z-Komprimierung. |

### Siehe auch

* namensraum [Aspose.Zip.Tar](../../aspose.zip.tar)
* Montage [Aspose.Zip](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
