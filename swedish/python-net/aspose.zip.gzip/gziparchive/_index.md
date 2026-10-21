---
title: "GzipArchive"
second_title: "Aspose.Zip för Python via .NET API-referens"
description: 
type: docs
weight: 10
url: /sv/python-net/aspose.zip.gzip/gziparchive/
---

## GzipArchive class

Denna klass representerar en gzip-arkivfil. Använd den för att skapa eller extrahera gzip-arkiv.

Typen GzipArchive exponerar följande medlemmar:
## Konstruktörer
| Namn | Beskrivning |
| :- | :- |
| GzipArchive() | Initierar en ny instans av klassen [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) för komprimering. |
| GzipArchive(source_stream, parse_header) | Initierar en ny instans av klassen [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) för dekomprimering. |
| GzipArchive(source_stream, options) | Initierar en ny instans av klassen [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) för dekomprimering. |
| GzipArchive(path, options) | Initierar en ny instans av klassen [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) för dekomprimering. |
| GzipArchive(path, parse_header) | Initierar en ny instans av klassen [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) för dekomprimering. |
## Egenskaper
| Namn | Beskrivning |
| :- | :- |
| uncompressed_size | Hämtar storleken på en originalfil. |
| name | Namnet på den ursprungliga filen. |
| file_entries | Hämtar poster av typen [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) som utgör arkivet. |
| format | Hämtar arkivformatet. |
| length | Hämtar längden på posten i byte. |
## Metoder
| Namn | Beskrivning |
| :- | :- |
| set_source(source) | Ställer in innehållet som ska komprimeras i arkivet. |
| set_source(file_info) | Ställer in innehållet som ska komprimeras i arkivet. |
| set_source(path) | Ställer in innehållet som ska komprimeras i arkivet. |
| set_source(tar_archive) | Ställer in innehållet som ska komprimeras i arkivet. |
| extract(destination) | Extraherar arkivet till den angivna strömmen. |
| extract(path) | Extraherar arkivets innehåll till den angivna katalogen. |
| save(output_stream) | Sparar arkivet till den angivna strömmen. |
| save(destination_file_name) | Sparar arkivet till den angivna destinationsfilen. |
| open() | Öppnar arkivet för extrahering och tillhandahåller en ström med arkivinnehållet. |
| extract_to_directory(destination_directory) | Extraherar arkivets innehåll till den angivna katalogen. |

### Se även

* namespace [aspose.zip.gzip](/zip/python-net/aspose.zip.gzip/)
* assembly [Aspose.Zip](/zip/python-net/)

