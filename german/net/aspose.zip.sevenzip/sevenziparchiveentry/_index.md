---
title: Class SevenZipArchiveEntry
second_title: Aspose.ZIP für .NET-API-Referenz
description: Aspose.Zip.SevenZip.SevenZipArchiveEntry klas. Stellt eine einzelne Datei innerhalb eines 7zArchivs dar.
type: docs
weight: 670
url: /de/net/aspose.zip.sevenzip/sevenziparchiveentry/
---
## SevenZipArchiveEntry class

Stellt eine einzelne Datei innerhalb eines 7z-Archivs dar.

```csharp
public abstract class SevenZipArchiveEntry : IArchiveFileEntry
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/compressedsize/) { get; } | Ruft die Größe der komprimierten Datei ab. |
| [CompressionSettings](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionsettings/) { get; } | Ruft Einstellungen für Komprimierung oder Dekomprimierung ab. |
| [IsDirectory](../../aspose.zip.sevenzip/sevenziparchiveentry/isdirectory/) { get; } | Ruft einen Wert ab, der angibt, ob der Eintrag ein Verzeichnis darstellt. |
| [ModificationTime](../../aspose.zip.sevenzip/sevenziparchiveentry/modificationtime/) { get; } | Ruft Datum und Uhrzeit der letzten Änderung ab. |
| [Name](../../aspose.zip.sevenzip/sevenziparchiveentry/name/) { get; } | Ruft den Namen des Eintrags im Archiv ab. |
| [UncompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/uncompressedsize/) { get; } | Ruft die Größe der Originaldatei ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract_1)(Stream, string) | Extrahiert den Eintrag zum bereitgestellten Stream. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract)(string, string) | Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit Eintragsinhalt bereit. |

## Veranstaltungen

| Name | Beschreibung |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | Wird ausgelöst, wenn ein Teil des Rohdatenstroms komprimiert wird. |

### Bemerkungen

Wirf ein`SevenZipArchiveEntry` Instanz zu[`SevenZipArchiveEntryEncrypted`](../sevenziparchiveentryencrypted/) um festzustellen, ob der Eintrag verschlüsselt ist oder nicht.

### Siehe auch

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namensraum [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* Montage [Aspose.Zip](../../)


