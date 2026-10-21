---
title: "XzArchive"
second_title: "Aspose.Zip för Python via .NET API-referens"
description: 
type: docs
weight: 10
url: /sv/python-net/aspose.zip.xz/xzarchive/
---

## XzArchive class

Denna klass representerar en xz-arkivfil. Använd den för att skapa och extrahera xz-arkiv.

Typen XzArchive exponerar följande medlemmar:
## Konstruktörer
| Namn | Beskrivning |
| :- | :- |
| XzArchive(settings) | Initierar en ny instans av klassen [XzArchive](/zip/python-net/aspose.zip.xz/xzarchive/) och skapar arkivet i xz-format. |
| XzArchive(source, options) | Initierar en ny instans av klassen [XzArchive](/zip/python-net/aspose.zip.xz/xzarchive/) för dekomprimering. |
| XzArchive(path, options) | Initierar en ny instans av klassen [XzArchive](/zip/python-net/aspose.zip.xz/xzarchive/) för dekomprimering. |
## Egenskaper
| Namn | Beskrivning |
| :- | :- |
| uncompressed_size | Okomprimerad storlek på fildata i byte. |
| file_entries | Hämtar poster av typen [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) som utgör arkivet. |
| format | Hämtar arkivformatet. |
| name | Hämtar namn på posten. |
| length | Hämtar längden på posten i byte. |
## Metoder
| Namn | Beskrivning |
| :- | :- |
| extract(destination) | Extraherar xz-arkivet till en ström. |
| extract(file_info) | Extraherar xz-arkivet till en fil. |
| extract(path) | Extraherar arkivets innehåll till den angivna katalogen. |
| set_source(source) | Ställer in innehållet som ska komprimeras i arkivet. |
| set_source(file_info) | Ställer in innehållet som ska komprimeras i arkivet. |
| set_source(source_path) | Ställer in innehållet som ska komprimeras i arkivet. |
| save(output) | Sparar xz-arkivet till den angivna strömmen. |
| save(destination_file_name) | Sparar xz-arkivet till den angivna målfilen. |
| extract_to_directory(destination_directory) | Extraherar arkivets innehåll till den angivna katalogen. |

### Se även

* namespace [aspose.zip.xz](/zip/python-net/aspose.zip.xz/)
* assembly [Aspose.Zip](/zip/python-net/)

