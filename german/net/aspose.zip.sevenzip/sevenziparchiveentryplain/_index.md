---
title: Class SevenZipArchiveEntryPlain
second_title: Aspose.ZIP für .NET-API-Referenz
description: Aspose.Zip.SevenZip.SevenZipArchiveEntryPlain klas. SevenZipEintrag der ohne Verschlüsselung komprimiert oder ohne Entschlüsselung dekomprimiert werden muss.
type: docs
weight: 690
url: /de/net/aspose.zip.sevenzip/sevenziparchiveentryplain/
---
## SevenZipArchiveEntryPlain class

SevenZip-Eintrag, der ohne Verschlüsselung komprimiert oder ohne Entschlüsselung dekomprimiert werden muss.

```csharp
public class SevenZipArchiveEntryPlain : SevenZipArchiveEntry
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
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/)(Stream, string) | Extrahiert den Eintrag zum bereitgestellten Stream. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/)(string, string) | Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit Eintragsinhalt bereit. |

## Veranstaltungen

| Name | Beschreibung |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | Wird ausgelöst, wenn ein Teil des Rohdatenstroms komprimiert wird. |

### Siehe auch

* class [SevenZipArchiveEntry](../sevenziparchiveentry/)
* namensraum [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* Montage [Aspose.Zip](../../)


