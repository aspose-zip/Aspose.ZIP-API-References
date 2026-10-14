---
title: "Klasse IsoArchive"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "Aspose.Zip.Iso.IsoArchive Klasse. Stellt ein ISO-Archiv ISO 9660 dar."
type: docs
weight: 570
url: /de/net/aspose.zip.iso/isoarchive/
---
## IsoArchive class

Stellt ein ISO-Archiv (ISO 9660) dar.

```csharp
public sealed class IsoArchive : IArchive
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [IsoArchive](isoarchive/#constructor)() | Initialisiert eine neue Instanz der `IsoArchive` Klasse und erstellt ein leeres ISO-Archiv zum Hinzufügen neuer Dateien und Verzeichnisse. |
| [IsoArchive](isoarchive/#constructor_1)(Stream, IsoLoadOptions) | Initialisiert eine neue Instanz der `IsoArchive` Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [IsoArchive](isoarchive/#constructor_2)(string, IsoLoadOptions) | Initialisiert eine neue Instanz der `IsoArchive` Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Entries](../../aspose.zip.iso/isoarchive/entries/) { get; } | Liefert Einträge des Typs [`IsoEntry`](../isoentry/), die das Archiv bilden. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [CreateDirectory](../../aspose.zip.iso/isoarchive/createdirectory/)(string) | Fügt dem ISO-Image ein Verzeichnis hinzu. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry)(string) | Fügt dem ISO-Image eine Datei hinzu. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_1)(string, Stream) | Fügt dem ISO-Image eine Datei hinzu. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_2)(string, string) | Fügt dem ISO-Image eine Datei hinzu. |
| [Dispose](../../aspose.zip.iso/isoarchive/dispose/)() | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [ExtractToDirectory](../../aspose.zip.iso/isoarchive/extracttodirectory/)(string) | Extrahiert alle Einträge in das angegebene Verzeichnis. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save)(Stream, IsoSaveOptions) | Speichert das ISO-Image in den angegebenen Stream. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save_1)(string, IsoSaveOptions) | Speichert das ISO-Image im angegebenen Pfad. |

### Siehe auch

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Iso](../../aspose.zip.iso/)
* assembly [Aspose.Zip](../../)


