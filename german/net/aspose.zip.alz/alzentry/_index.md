---
title: "Klasse AlzEntry"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "Aspose.Zip.Alz.AlzEntry Klasse. Stellt einen Dateieintrag in einem ALZ-Archiv mit allen Metadaten dar"
type: docs
weight: 30
url: /de/net/aspose.zip.alz/alzentry/
---
## AlzEntry class

Stellt einen Dateieintrag in einem ALZ-Archiv mit allen Metadaten dar.

```csharp
public abstract class AlzEntry : IArchiveFileEntry
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CompressedSize](../../aspose.zip.alz/alzentry/compressedsize/) { get; } | Komprimierte Größe der Dateidaten in Bytes. |
| [IsDirectory](../../aspose.zip.alz/alzentry/isdirectory/) { get; } | Gibt true zurück, wenn dieser Eintrag ein Verzeichnis darstellt. |
| [Length](../../aspose.zip.alz/alzentry/length/) { get; } |  |
| [Name](../../aspose.zip.alz/alzentry/name/) { get; } | Dateiname (ohne Pfad). |
| [UncompressedSize](../../aspose.zip.alz/alzentry/uncompressedsize/) { get; } | Unkomprimierte Größe der Dateidaten in Bytes. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract_1)(Stream, string) | Extrahiert den Eintrag in den bereitgestellten Stream. |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract)(string, string) | Extrahiert den Eintrag in das Dateisystem anhand des angegebenen Pfads. |
| [Open](../../aspose.zip.alz/alzentry/open/)(string) | Öffnet den Eintrag zum Extrahieren und liefert einen Stream mit dem dekomprimierten Eintragsinhalt. |

### Siehe auch

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Alz](../../aspose.zip.alz/)
* assembly [Aspose.Zip](../../)


