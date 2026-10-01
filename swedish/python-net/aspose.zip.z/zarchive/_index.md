---
title: "ZArchive"
second_title: "Aspose.Zip för Python via .NET API-referens"
description: 
type: docs
weight: 10
url: /sv/python-net/aspose.zip.z/zarchive/
---

## ZArchive class

Denna klass representerar en Z (compress) arkivfil. Använd den för att skapa eller extrahera Z-arkiv.

Typen ZArchive exponerar följande medlemmar:
## Konstruktörer
| Namn | Beskrivning |
| :- | :- |
| ZArchive() | Initierar en ny instans av klassen [ZArchive](/zip/python-net/aspose.zip.z/zarchive/) för komprimering. |
| ZArchive(source, load_options) | Initierar en ny instans av klassen [ZArchive](/zip/python-net/aspose.zip.z/zarchive/) för dekomprimering. |
| ZArchive(path, load_options) | Initierar en ny instans av klassen [ZArchive](/zip/python-net/aspose.zip.z/zarchive/) för dekomprimering. |
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
| extract(destination) | Extraherar Z-arkivet till en ström. |
| extract(file_info) | Extraherar Z-arkivet till en fil. |
| extract(path) | Extraherar Z-arkivet till en fil via sökväg. |
| save(output, settings) | Sparar xz-arkivet till den angivna strömmen. |
| save(destination_file_name, settings) | Sparar Z-arkivet till den angivna destinationsfilen. |
| set_source(source) | Ställer in innehållet som ska komprimeras i arkivet. |
| set_source(file_info) | Ställer in innehållet som ska komprimeras i arkivet. |
| set_source(source_path) | Ställer in innehållet som ska komprimeras i arkivet. |
| extract_to_directory(destination_directory) | Extraherar arkivets innehåll till den angivna katalogen. |

### Se även

* namespace [aspose.zip.z](/zip/python-net/aspose.zip.z/)
* assembly [Aspose.Zip](/zip/python-net/)

