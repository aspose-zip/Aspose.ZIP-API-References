---
title: "Klasse ArjArchive"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "Aspose.Zip.Arj.ArjArchive‑Klasse. Diese Klasse stellt eine ARJ‑Archivdatei dar."
type: docs
weight: 250
url: /de/net/aspose.zip.arj/arjarchive/
---
## ArjArchive class

Diese Klasse repräsentiert eine ARJ-Archivdatei.

```csharp
public class ArjArchive : IArchive
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [ArjArchive](arjarchive/#constructor)(Stream, ArjLoadOptions) | Initialisiert eine neue Instanz der `ArjArchive`‑Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [ArjArchive](arjarchive/#constructor_1)(string, ArjLoadOptions) | Initialisiert eine neue Instanz der `ArjArchive`‑Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Commentary](../../aspose.zip.arj/arjarchive/commentary/) { get; } | Liest den Kommentar. |
| [Entries](../../aspose.zip.arj/arjarchive/entries/) { get; } | Liest Einträge des Typs [`ArjEntryPlain`](../arjentryplain/), die das ARJ‑Archiv bilden. |
| [Name](../../aspose.zip.arj/arjarchive/name/) { get; } | Liest den ursprünglichen Namen. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Dispose](../../aspose.zip.arj/arjarchive/dispose/)() | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [ExtractToDirectory](../../aspose.zip.arj/arjarchive/extracttodirectory/)(string) | Extrahiert alle Einträge in das angegebene Verzeichnis. |

## Hinweise

Nur die folgenden Komprimierungsmethoden werden unterstützt:

**Method**

**Explanation**

**0**

Unkomprimiert

**1**

Kombination aus LZ77 und adaptiver Huffman‑Codierung. Bestes Kompressionsverhältnis.

**2**

Kombination aus LZ77 und adaptiver Huffman‑Codierung.

**3**

Kombination aus LZ77 und adaptiver Huffman‑Codierung. Schnellste Geschwindigkeit.

### Siehe auch

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Arj](../../aspose.zip.arj/)
* assembly [Aspose.Zip](../../)


