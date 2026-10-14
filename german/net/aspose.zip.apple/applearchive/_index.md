---
title: "Klasse AppleArchive"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "Aspose.Zip.Apple.AppleArchive Klasse. Diese Klasse repräsentiert eine Apple Archive .aar Datei. Verwenden Sie sie, um Apple Archive-Dateien zu erstellen."
type: docs
weight: 60
url: /de/net/aspose.zip.apple/applearchive/
---
## AppleArchive class

Diese Klasse repräsentiert eine Apple Archive (.aar)-Datei. Verwenden Sie sie zum Erstellen von Apple Archive-Dateien.

```csharp
public class AppleArchive : IArchive
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [AppleArchive](applearchive/#constructor)(AppleArchiveEntrySettings) | Initialisiert eine neue Instanz der `AppleArchive`-Klasse mit den für zusammengesetzte Einträge verwendeten Einstellungen. |
| [AppleArchive](applearchive/#constructor_1)(Stream, AppleArchiveLoadOptions) | Initialisiert eine neue Instanz der `AppleArchive`-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [AppleArchive](applearchive/#constructor_2)(string, AppleArchiveLoadOptions) | Initialisiert eine neue Instanz der `AppleArchive`-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Entries](../../aspose.zip.apple/applearchive/entries/) { get; } | Liefert die Einträge, aus denen das Archiv besteht. |
| [IsSolid](../../aspose.zip.apple/applearchive/issolid/) { get; } | Gibt einen Wert zurück, der angibt, ob das Archiv eine Solid‑Kompression verwendet. Im Solid‑Modus werden alle Eintragsdaten als ein einziger Strom komprimiert und eine einzelne Eintrags‑Extraktion ist nicht verfügbar. Verwenden Sie stattdessen [`ExtractToDirectory`](../../aspose.zip/iarchive/extracttodirectory/). |
| [NewEntrySettings](../../aspose.zip.apple/applearchive/newentrysettings/) { get; } | Liefert die für neu erstellte Einträge verwendeten Einstellungen. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [CreateEntries](../../aspose.zip.apple/applearchive/createentries/)(DirectoryInfo, bool) | Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv aus dem angegebenen Verzeichnis hinzu. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_1)(string, Stream) | Erstellt einen einzelnen Eintrag im Archiv. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry)(string, FileInfo, bool) | Erstellt einen einzelnen Eintrag im Archiv. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_2)(string, string, bool) | Erstellt einen einzelnen Eintrag im Archiv. |
| [Dispose](../../aspose.zip.apple/applearchive/dispose/)() | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [ExtractToDirectory](../../aspose.zip.apple/applearchive/extracttodirectory/)(string) | Extrahiert alle Dateien im Archiv in das angegebene Verzeichnis. |
| [Save](../../aspose.zip.apple/applearchive/save/#save)(Stream) | Speichert das Archiv in den bereitgestellten Stream. |
| [Save](../../aspose.zip.apple/applearchive/save/#save_1)(string) | Speichert das Archiv in eine bereitgestellte Zieldatei. |

## Hinweise

Apple und Apple Archive sind Marken von Apple Inc.

### Siehe auch

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


