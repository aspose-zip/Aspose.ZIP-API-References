---
title: "Archive"
second_title: "Aspose.Zip för Python via .NET API-referens"
description: 
type: docs
weight: 10
url: /sv/python-net/aspose.zip/archive/
---

## Archive class

Denna klass representerar en zip-arkivfil. Använd den för att skapa, extrahera eller uppdatera zip-arkiv.

Typen Archive visar följande medlemmar:
## Konstruktörer
| Namn | Beskrivning |
| :- | :- |
| Archive(new_entry_settings) | Initierar en ny instans av klassen [Archive](/zip/python-net/aspose.zip/archive/) med valfria inställningar för dess poster. |
| Archive(source_stream, load_options, new_entry_settings) | Initierar en ny instans av klassen [Archive](/zip/python-net/aspose.zip/archive/) och samlar en postlista som kan extraheras från arkivet. |
| Archive(path, load_options, new_entry_settings) | Initierar en ny instans av klassen [Archive](/zip/python-net/aspose.zip/archive/) och samlar en postlista som kan extraheras från arkivet. |
| Archive(main_segment, segments_in_order, load_options) | Initierar en ny instans av klassen [Archive](/zip/python-net/aspose.zip/archive/) från ett flervolymigt ZIP-arkiv och skapar en postlista som kan extraheras från arkivet. |
## Egenskaper
| Namn | Beskrivning |
| :- | :- |
| new_entry_settings | Komprimerings- och krypteringsinställningar som används för nyss tillagda [ArchiveEntry](/zip/python-net/aspose.zip/archiveentry/) objekt. |
| comment | Hämtar kommentar för hela arkivet. |
| entries | Hämtar poster av typen [ArchiveEntry](/zip/python-net/aspose.zip/archiveentry/) som utgör arkivet. |
| file_entries | Hämtar poster av typen [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) som utgör arkivet. |
| format | Hämtar arkivformatet. |
## Metoder
| Namn | Beskrivning |
| :- | :- |
| create_entry(name, path, open_immediately, new_entry_settings) | Skapa en enskild post i arkivet. |
| create_entry(name, source, new_entry_settings) | Skapa en enskild post i arkivet. |
| create_entry(name, file_info, open_immediately, new_entry_settings) | Skapa en enskild post i arkivet. |
| create_entry(name, source, new_entry_settings, file_info) | Skapa en enskild post i arkivet. |
| create_entries(directory, include_root_directory) | Lägg till alla filer och kataloger rekursivt i den angivna katalogen i arkivet. |
| create_entries(source_directory, include_root_directory) | Lägg till alla filer och kataloger rekursivt i den angivna katalogen i arkivet. |
| delete_entry(entry) | Tar bort den första förekomsten av den specifika posten från postlistan. |
| delete_entry(entry_index) |  |
| save(output_stream, save_options) | Sparar arkivet till den angivna strömmen. |
| save(destination_file_name, save_options) | Sparar arkivet till den angivna destinationsfilen. |
| save_split(destination_directory, options) | Sparar flervolymigt arkiv till den angivna destinationskatalogen. |
| extract_to_directory(destination_directory) | Extraherar alla filer i arkivet till den angivna katalogen. |

### Se även

* namespace [aspose.zip](/zip/python-net/aspose.zip/)
* assembly [Aspose.Zip](/zip/python-net/)

