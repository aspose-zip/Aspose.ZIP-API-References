---
title: "LzipArchive"
second_title: "Aspose.Zip för Python via .NET API-referens"
description: 
type: docs
weight: 10
url: /sv/python-net/aspose.zip.lzip/lziparchive/
---

## LzipArchive class

Denna klass representerar en Lzip-arkivfil. Använd den för att skapa eller extrahera Lzip-arkiv.

Typen LzipArchive exponerar följande medlemmar:
## Konstruktörer
| Namn | Beskrivning |
| :- | :- |
| LzipArchive(settings) | Initierar en ny instans av [LzipArchive](/zip/python-net/aspose.zip.lzip/lziparchive/). |
| LzipArchive(source_stream, options) | Initierar en ny instans av klassen [LzipArchive](/zip/python-net/aspose.zip.lzip/lziparchive/) för dekomprimering. |
| LzipArchive(path, options) | Initierar en ny instans av klassen [LzipArchive](/zip/python-net/aspose.zip.lzip/lziparchive/) för dekomprimering. |
## Egenskaper
| Namn | Beskrivning |
| :- | :- |
| uncompressed_size | Okomprimerad storlek på fildata i byte. |
| inställningar | Hämtar inställningen för ett specifikt lzip-arkiv. |
| file_entries | Hämtar poster av typen [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) som utgör arkivet. |
| format | Hämtar arkivformatet. |
| name | Hämtar namn på posten. |
| length | Hämtar längden på posten i byte. |
## Metoder
| Namn | Beskrivning |
| :- | :- |
| extract(destination) | Extraherar lzip-arkivet till en ström. |
| extract(file_info) | Extraherar lzip-arkivet till en fil. |
| extract(path) | Extraherar lzip-arkivet till en fil enligt sökväg. |
| save(output_stream) | Sparar lzip-arkivet till den angivna strömmen. |
| save(destination_file_name) | Sparar lzip-arkivet till den angivna destinationsfilen. |
| save(destination) | Sparar lzip-arkivet till den angivna destinationsfilen. |
| set_source(source) | Ställer in innehållet som ska komprimeras i arkivet. |
| set_source(file_info) | Ställer in innehållet som ska komprimeras i arkivet. |
| set_source(path) | Ställer in innehållet som ska komprimeras i arkivet. |
| extract_to_directory(destination_directory) | Extraherar arkivets innehåll till den angivna katalogen. |

### Se även

* namespace [aspose.zip.lzip](/zip/python-net/aspose.zip.lzip/)
* assembly [Aspose.Zip](/zip/python-net/)

