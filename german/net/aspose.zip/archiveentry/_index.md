---
title: Class ArchiveEntry
second_title: Aspose.ZIP für .NET-API-Referenz
description: Aspose.Zip.ArchiveEntry klas. Stellt eine einzelne Datei im Archiv dar.
type: docs
weight: 20
url: /de/net/aspose.zip/archiveentry/
---
## ArchiveEntry class

Stellt eine einzelne Datei im Archiv dar.

```csharp
public abstract class ArchiveEntry : IArchiveFileEntry
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | Ruft den Kommentar des Eintrags im Archiv ab. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | Ruft die Größe der komprimierten Datei ab. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | Ruft Einstellungen für Komprimierung oder Dekomprimierung ab. |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | Ruft einen Wert ab, der angibt, ob der Eintrag ein Verzeichnis darstellt. |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | Ruft Datum und Uhrzeit der letzten Änderung ab oder legt sie fest. |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | Ruft den Namen des Eintrags im Archiv ab. |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | Ruft die Größe der Originaldatei ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/#extract_1)(Stream, string) | Extrahiert den Eintrag zum bereitgestellten Stream. |
| [Extract](../../aspose.zip/archiveentry/extract/#extract)(string, string) | Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit dekomprimiertem Eintragsinhalt bereit. |

## Veranstaltungen

| Name | Beschreibung |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Wird ausgelöst, wenn ein Teil des Rohdatenstroms komprimiert wird. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Wird ausgelöst, wenn ein Teil des Rohdatenstroms extrahiert wird. |

### Bemerkungen

Wirf ein`ArchiveEntry` Instanz zu[`ArchiveEntryEncrypted`](../archiveentryencrypted/) um festzustellen, ob der Eintrag verschlüsselt ist oder nicht.

### Siehe auch

* interface [IArchiveFileEntry](../iarchivefileentry/)
* namensraum [Aspose.Zip](../../aspose.zip/)
* Montage [Aspose.Zip](../../)


