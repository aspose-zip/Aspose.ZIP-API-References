---
title: "Bzip2Archive"
second_title: "Aspose.Zip för Python via .NET API-referens"
description: 
type: docs
weight: 10
url: /sv/python-net/aspose.zip.bzip2/bzip2archive/
---

## Bzip2Archive class

Denna klass representerar en bzip2-arkivfil. Använd den för att skapa eller extrahera bzip2-arkiv.

Typen Bzip2Archive visar följande medlemmar:
## Konstruktörer
| Namn | Beskrivning |
| :- | :- |
| Bzip2Archive() | Initierar en ny instans av klassen [Bzip2Archive](/zip/python-net/aspose.zip.bzip2/bzip2archive/) för komprimering. |
| Bzip2Archive(source_stream, load_options) | Initierar en ny instans av klassen [Bzip2Archive](/zip/python-net/aspose.zip.bzip2/bzip2archive/) för dekomprimering. |
| Bzip2Archive(path, load_options) | Initierar en ny instans av klassen [Bzip2Archive](/zip/python-net/aspose.zip.bzip2/bzip2archive/) för dekomprimering. |
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
| set_source(source) | Ställer in innehållet som ska komprimeras i arkivet. |
| set_source(file_info) | Ställer in innehållet som ska komprimeras i arkivet. |
| set_source(path) | Ställer in innehållet som ska komprimeras i arkivet. |
| set_source(tar_archive, format) | Ställer in innehållet som ska komprimeras i arkivet. |
| set_source(cpio_archive, format) | Ställer in innehållet som ska komprimeras i arkivet. |
| extract(destination) | Extraherar arkivet till den angivna strömmen. |
| extract(path) | Extraherar arkivets innehåll till den angivna katalogen. |
| save(output_stream, save_options) | Sparar arkivet till den angivna strömmen. |
| save(destination_file_name, save_options) | Sparar arkivet till den angivna destinationsfilen. |
| open() | Öppnar arkivet för extrahering och tillhandahåller en ström med arkivinnehållet. |
| extract_to_directory(destination_directory) | Extraherar arkivets innehåll till den angivna katalogen. |

### Se även

* namespace [aspose.zip.bzip2](/zip/python-net/aspose.zip.bzip2/)
* assembly [Aspose.Zip](/zip/python-net/)

