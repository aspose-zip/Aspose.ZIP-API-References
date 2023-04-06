---
title: Class GzipArchive
second_title: Aspose.ZIP voor .NET API-referentie
description: Aspose.Zip.Gzip.GzipArchive klas. Deze klasse vertegenwoordigt het gziparchiefbestand. Gebruik het om gziparchieven samen te stellen of uit te pakken.
type: docs
weight: 210
url: /nl/net/aspose.zip.gzip/gziparchive/
---
## GzipArchive class

Deze klasse vertegenwoordigt het gzip-archiefbestand. Gebruik het om gzip-archieven samen te stellen of uit te pakken.

```csharp
public class GzipArchive : IArchive, IArchiveFileEntry
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [GzipArchive](gziparchive/#constructor)() | Initialiseert een nieuw exemplaar van het`GzipArchive` klasse voorbereid voor compressie. |
| [GzipArchive](gziparchive/#constructor_1)(Stream, bool) | Initialiseert een nieuw exemplaar van het`GzipArchive` klasse voorbereid voor decomprimeren. |
| [GzipArchive](gziparchive/#constructor_2)(string, bool) | Initialiseert een nieuw exemplaar van het`GzipArchive` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Name](../../aspose.zip.gzip/gziparchive/name/) { get; } | Naam van origineel bestand. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| [Dispose](../../aspose.zip.gzip/gziparchive/dispose/)() | Voert door de toepassing gedefinieerde taken uit die verband houden met het vrijmaken, vrijgeven of resetten van onbeheerde bronnen. |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/)(Stream) | Pakt het archief uit naar de geleverde stream. |
| [Open](../../aspose.zip.gzip/gziparchive/open/)() | Opent het archief voor extractie en levert een stream met archiefinhoud. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save)(Stream) | Slaat archief op in de geleverde stream. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save_1)(string) | Slaat archief op in opgegeven bestemmingsbestand. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_1)(FileInfo) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_2)(Stream) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_3)(string) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource)(TarArchive) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |

### Opmerkingen

Het Gzip-compressiealgoritme is gebaseerd op het DEFLATE-algoritme, een combinatie van LZ77- en Huffman-codering.

### Zie ook

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* naamruimte [Aspose.Zip.Gzip](../../aspose.zip.gzip/)
* montage [Aspose.Zip](../../)


