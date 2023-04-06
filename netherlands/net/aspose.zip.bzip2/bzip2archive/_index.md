---
title: Class Bzip2Archive
second_title: Aspose.ZIP voor .NET API-referentie
description: Aspose.Zip.Bzip2.Bzip2Archive klas. Deze klasse vertegenwoordigt het bzip2archiefbestand. Gebruik het om bzip2archieven samen te stellen of uit te pakken.
type: docs
weight: 100
url: /nl/net/aspose.zip.bzip2/bzip2archive/
---
## Bzip2Archive class

Deze klasse vertegenwoordigt het bzip2-archiefbestand. Gebruik het om bzip2-archieven samen te stellen of uit te pakken.

```csharp
public class Bzip2Archive : IArchive, IArchiveFileEntry
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [Bzip2Archive](bzip2archive/#constructor)() | Initialiseert een nieuw exemplaar van het`Bzip2Archive` klasse voorbereid voor compressie. |
| [Bzip2Archive](bzip2archive/#constructor_1)(Stream) | Initialiseert een nieuw exemplaar van het`Bzip2Archive` klasse voorbereid voor decomprimeren. |
| [Bzip2Archive](bzip2archive/#constructor_2)(string) | Initialiseert een nieuw exemplaar van het`Bzip2Archive` klasse voorbereid voor decomprimeren. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| [Dispose](../../aspose.zip.bzip2/bzip2archive/dispose/)() | Voert door de toepassing gedefinieerde taken uit die verband houden met het vrijmaken, vrijgeven of resetten van onbeheerde bronnen. |
| [Extract](../../aspose.zip.bzip2/bzip2archive/extract/)(Stream) | Pakt het archief uit naar de geleverde stream. |
| [Open](../../aspose.zip.bzip2/bzip2archive/open/)() | Opent het archief voor extractie en levert een stream met archiefinhoud. |
| [Save](../../aspose.zip.bzip2/bzip2archive/save/#save)(Stream, Bzip2SaveOptions) | Slaat archief op in de geleverde stream. |
| [Save](../../aspose.zip.bzip2/bzip2archive/save/#save_1)(string, Bzip2SaveOptions) | Slaat archief op in opgegeven bestemmingsbestand. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_2)(FileInfo) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_3)(Stream) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_4)(string) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource)(CpioArchive, CpioFormat) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_1)(TarArchive, TarFormat) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |

### Opmerkingen

bzip2 comprimeert bestanden met behulp van het Burrows-Wheeler block sorting tekstcompressie-algoritme en Huffman-codering. Zie meer: https://en.wikipedia.org/wiki/Bzip2

### Zie ook

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* naamruimte [Aspose.Zip.Bzip2](../../aspose.zip.bzip2/)
* montage [Aspose.Zip](../../)


