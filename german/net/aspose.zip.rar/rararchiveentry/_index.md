---
title: Class RarArchiveEntry
second_title: Aspose.ZIP für .NET-API-Referenz
description: Aspose.Zip.Rar.RarArchiveEntry klas. Stellt eine einzelne Datei im Archiv dar.
type: docs
weight: 320
url: /de/net/aspose.zip.rar/rararchiveentry/
---
## RarArchiveEntry class

Stellt eine einzelne Datei im Archiv dar.

```csharp
public abstract class RarArchiveEntry : IArchiveFileEntry
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CompressedSize](../../aspose.zip.rar/rararchiveentry/compressedsize/) { get; } | Ruft die Größe der komprimierten Datei ab. |
| [CreationTime](../../aspose.zip.rar/rararchiveentry/creationtime/) { get; } | Ruft Erstellungsdatum und -zeit ab. |
| [IsDirectory](../../aspose.zip.rar/rararchiveentry/isdirectory/) { get; } | Ruft einen Wert ab, der angibt, ob der Eintrag ein Verzeichnis darstellt. |
| [LastAccessTime](../../aspose.zip.rar/rararchiveentry/lastaccesstime/) { get; } | Ruft Datum und Uhrzeit des letzten Zugriffs ab. |
| [ModificationTime](../../aspose.zip.rar/rararchiveentry/modificationtime/) { get; } | Ruft Datum und Uhrzeit der letzten Änderung ab. |
| [Name](../../aspose.zip.rar/rararchiveentry/name/) { get; } | Ruft den Namen des Eintrags im Archiv ab. |
| [UncompressedSize](../../aspose.zip.rar/rararchiveentry/uncompressedsize/) { get; } | Ruft die Größe der Originaldatei ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract_1)(Stream, string) | Extrahiert den Eintrag zum bereitgestellten Stream. |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract)(string, string) | Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad. |
| [Open](../../aspose.zip.rar/rararchiveentry/open/)(string) | Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit dekomprimiertem Eintragsinhalt bereit. |

## Veranstaltungen

| Name | Beschreibung |
| --- | --- |
| event [ExtractionProgressed](../../aspose.zip.rar/rararchiveentry/extractionprogressed/) | Wird ausgelöst, wenn ein Teil des Rohdatenstroms extrahiert wird. |

### Bemerkungen

Cast a`RarArchiveEntry` Instanz zu[`RarArchiveEntryEncrypted`](../rararchiveentryencrypted/) um festzustellen, ob der Eintrag verschlüsselt ist oder nicht.

### Siehe auch

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namensraum [Aspose.Zip.Rar](../../aspose.zip.rar/)
* Montage [Aspose.Zip](../../)


