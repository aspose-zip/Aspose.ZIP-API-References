---
title: "Klasse LhaArchive"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "**Aspose.Zip.Lha.LhaArchive** Klasse. Diese Klasse repräsentiert eine LHA .lzh-Archivdatei"
type: docs
weight: 630
url: /de/net/aspose.zip.lha/lhaarchive/
---
## LhaArchive class

Diese Klasse repräsentiert eine LHA (.lzh)-Archivdatei.

```csharp
public class LhaArchive : IArchive
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [LhaArchive](lhaarchive/#constructor)(Stream, LhaLoadOptions) | Initialisiert eine neue Instanz der `LhaArchive` Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [LhaArchive](lhaarchive/#constructor_1)(string, LhaLoadOptions) | Initialisiert eine neue Instanz der `LhaArchive` Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Entries](../../aspose.zip.lha/lhaarchive/entries/) { get; } | Ermittelt Dateieinträge des Typs [`LhaArchiveEntry`](../lhaarchiveentry/), die das Archiv bilden. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Dispose](../../aspose.zip.lha/lhaarchive/dispose/)() |  |
| [ExtractToDirectory](../../aspose.zip.lha/lhaarchive/extracttodirectory/)(string) | Extrahiert alle Dateien und Verzeichnisse im Archiv in das angegebene Verzeichnis. |

## Hinweise

Nur die folgenden Komprimierungsmethoden werden unterstützt:

**Method**

**Explanation**

**lh0**

Unkomprimiert

**lh4**

8 KiB Gleitendes Wörterbuch und statisches Huffman

**lh5**

16 KiB Gleitendes Wörterbuch und statisches Huffman

**lh6**

64 KiB Gleitendes Wörterbuch und statisches Huffman

**lh7**

128 KiB Gleitendes Wörterbuch und statisches Huffman

**lhx**

1 Mib Gleitendes Wörterbuch und statisches Huffman

**lhd**

Verzeichnis

### Siehe auch

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Lha](../../aspose.zip.lha/)
* assembly [Aspose.Zip](../../)


