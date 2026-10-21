---
title: "CabArchive"
second_title: "Aspose.Zip för Python via .NET API-referens"
description: 
type: docs
weight: 10
url: /sv/python-net/aspose.zip.cab/cabarchive/
---

## CabArchive class

Denna klass representerar en CAB-arkivfil.

Typen CabArchive exponerar följande medlemmar:
## Konstruktörer
| Namn | Beskrivning |
| :- | :- |
| CabArchive(settings) | Initierar en ny instans av klassen [CabArchive](/zip/python-net/aspose.zip.cab/cabarchive/) för komprimering. |
| CabArchive(source_stream, load_options) | Initierar en ny instans av klassen [CabArchive](/zip/python-net/aspose.zip.cab/cabarchive/) och skapar en postlista som kan extraheras från arkivet. |
| CabArchive(path, load_options) | Initierar en ny instans av klassen [CabArchive](/zip/python-net/aspose.zip.cab/cabarchive/) och skapar en postlista som kan extraheras från arkivet. |
## Egenskaper
| Namn | Beskrivning |
| :- | :- |
| entries | Hämtar poster av typen [CabEntry](/zip/python-net/aspose.zip.cab/cabentry/) som utgör arkivet. |
| file_entries | Hämtar poster av typen [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) som utgör arkivet. |
| format | Hämtar arkivformatet. |
## Metoder
| Namn | Beskrivning |
| :- | :- |
| create_entry(name, path, new_entry_settings) | Skapa en enskild post i arkivet. |
| create_entry(name, source, new_entry_settings) | Skapa en enskild post i arkivet. |
| create_entry(name, file_info, new_entry_settings) | Skapa en enskild post i arkivet. |
| create_entries(directory, include_root_directory) | Lägger till alla filer, rekursivt, från den angivna katalogen till arkivet. |
| create_entries(source_directory, include_root_directory) | Lägger till alla filer rekursivt från den angivna katalogsökvägen till arkivet. |
| save(output_stream, save_options) | Sparar arkivet till den angivna strömmen. |
| save(destination_file_name, save_options) | Sparar arkivet till den angivna destinationsfilen. |
| extract_to_directory(destination_directory) | Extraherar alla filer i arkivet till den angivna katalogen. |

### Se även

* namespace [aspose.zip.cab](/zip/python-net/aspose.zip.cab/)
* assembly [Aspose.Zip](/zip/python-net/)

