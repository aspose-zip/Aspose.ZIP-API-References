---
title: "ZstandardArchive"
second_title: "Aspose.Zip för Python via .NET API-referens"
description: 
type: docs
weight: 10
url: /sv/python-net/aspose.zip.zstandard/zstandardarchive/
---

## ZstandardArchive class

Denna klass representerar en Zstandard-arkivfil. Använd den för att skapa Zstandard-arkiv.

Typen ZstandardArchive visar följande medlemmar:
## Konstruktörer
| Namn | Beskrivning |
| :- | :- |
| ZstandardArchive() | Initierar en ny instans av klassen [ZstandardArchive](/zip/python-net/aspose.zip.zstandard/zstandardarchive/) för komprimering. |
| ZstandardArchive(source_stream, options) | Initierar en ny instans av klassen [ZstandardArchive](/zip/python-net/aspose.zip.zstandard/zstandardarchive/) för dekomprimering. |
| ZstandardArchive(path, options) | Initierar en ny instans av klassen [ZstandardArchive](/zip/python-net/aspose.zip.zstandard/zstandardarchive/). |
## Egenskaper
| Namn | Beskrivning |
| :- | :- |
| file_entries | Hämtar poster av typen [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) som utgör arkivet. |
| format | Hämtar arkivformatet. |
| name | Hämtar namn på posten. |
| length | Hämtar längden på posten i byte. |
## Metoder
| Namn | Beskrivning |
| :- | :- |
| extract(destination) | Extraherar arkivet till den angivna strömmen. |
| extract(path) | Extraherar arkivet till filen enligt sökväg. |
| set_source(source) | Ställer in innehållet som ska komprimeras i arkivet. |
| set_source(file_info) | Ställer in innehållet som ska komprimeras i arkivet. |
| set_source(path) | Ställer in innehållet som ska komprimeras i arkivet. |
| save(output_stream, settings) | Sparar arkivet till den angivna strömmen. |
| save(destination_file_name, settings) | Sparar arkivet till den angivna destinationsfilen. |
| save(destination, settings) | Sparar arkivet till den angivna destinationsfilen. |
| open() | Öppnar arkivet för extrahering och tillhandahåller en ström med arkivinnehållet. |
| extract_to_directory(destination_directory) | Extraherar arkivets innehåll till den angivna katalogen. |

### Se även

* namespace [aspose.zip.zstandard](/zip/python-net/aspose.zip.zstandard/)
* assembly [Aspose.Zip](/zip/python-net/)

