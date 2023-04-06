---
title: Class ArchiveEntryEncrypted
second_title: Aspose.ZIP für .NET-API-Referenz
description: Aspose.Zip.ArchiveEntryEncrypted klas. ZipEintrag der mit Verschlüsselung komprimiert oder mit Entschlüsselung dekomprimiert werden muss.
type: docs
weight: 30
url: /de/net/aspose.zip/archiveentryencrypted/
---
## ArchiveEntryEncrypted class

Zip-Eintrag, der mit Verschlüsselung komprimiert oder mit Entschlüsselung dekomprimiert werden muss.

```csharp
public sealed class ArchiveEntryEncrypted : ArchiveEntry
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | Ruft den Kommentar des Eintrags im Archiv ab. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | Ruft die Größe der komprimierten Datei ab. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | Ruft Einstellungen für Komprimierung oder Dekomprimierung ab. |
| [EncryptionSettings](../../aspose.zip/archiveentryencrypted/encryptionsettings/) { get; } | Ruft Einstellungen für die Verschlüsselung oder Entschlüsselung ab. |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | Ruft einen Wert ab, der angibt, ob der Eintrag ein Verzeichnis darstellt. |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | Ruft Datum und Uhrzeit der letzten Änderung ab oder legt sie fest. |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | Ruft den Namen des Eintrags im Archiv ab. |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | Ruft die Größe der Originaldatei ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/)(Stream, string) | Extrahiert den Eintrag zum bereitgestellten Stream. |
| [Extract](../../aspose.zip/archiveentry/extract/)(string, string) | Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit dekomprimiertem Eintragsinhalt bereit. |

## Veranstaltungen

| Name | Beschreibung |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Wird ausgelöst, wenn ein Teil des Rohdatenstroms komprimiert wird. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Wird ausgelöst, wenn ein Teil des Rohdatenstroms extrahiert wird. |

### Siehe auch

* class [ArchiveEntry](../archiveentry/)
* namensraum [Aspose.Zip](../../aspose.zip/)
* Montage [Aspose.Zip](../../)


