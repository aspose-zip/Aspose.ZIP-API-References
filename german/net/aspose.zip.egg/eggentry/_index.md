---
title: "Klasse EggEntry"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "Aspose.Zip.Egg.EggEntry class. Stellt einen Dateieintrag in einem EGG-Archiv mit allen zugehörigen Metadaten dar"
type: docs
weight: 470
url: /de/net/aspose.zip.egg/eggentry/
---
## EggEntry class

Stellt einen Dateieintrag in einem EGG-Archiv mit allen Metadaten dar.

```csharp
public abstract class EggEntry : IArchiveFileEntry
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CompressedSize](../../aspose.zip.egg/eggentry/compressedsize/) { get; } | Liefert die komprimierte Größe des Eintrags. |
| [IsDirectory](../../aspose.zip.egg/eggentry/isdirectory/) { get; } | Gibt einen Wert zurück, der angibt, ob dieser Eintrag ein Verzeichnis darstellt. |
| [Length](../../aspose.zip.egg/eggentry/length/) { get; } |  |
| [ModificationTime](../../aspose.zip.egg/eggentry/modificationtime/) { get; } | Liest oder setzt das Datum und die Uhrzeit der letzten Änderung. |
| [Name](../../aspose.zip.egg/eggentry/name/) { get; } | Liefert den Namen des Eintrags im Archiv. |
| [UncompressedSize](../../aspose.zip.egg/eggentry/uncompressedsize/) { get; } | Liefert die unkomprimierte Größe des Eintrags. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract_1)(Stream) | Extrahiert den Eintrag in den bereitgestellten Stream. |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract)(string) | Extrahiert den Eintrag in das Dateisystem anhand des angegebenen Pfads. |
| [Open](../../aspose.zip.egg/eggentry/open/)() | Öffnet den Eintrag zum Extrahieren und liefert einen Stream mit dem dekomprimierten Eintragsinhalt. |

### Siehe auch

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Egg](../../aspose.zip.egg/)
* assembly [Aspose.Zip](../../)


