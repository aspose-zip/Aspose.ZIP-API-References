---
title: "AppleArchive"
second_title: "Aspose.Zip för Python via .NET API-referens"
description: 
type: docs
weight: 10
url: /sv/python-net/aspose.zip.apple/applearchive/
---

## AppleArchive class

Denna klass representerar en Apple Archive (.aar)-fil. Använd den för att skapa Apple Archive-filer.

Typen AppleArchive exponerar följande medlemmar:
## Konstruktörer
| Namn | Beskrivning |
| :- | :- |
| AppleArchive(new_entry_settings) | Initierar en ny instans av klassen [AppleArchive](/zip/python-net/aspose.zip.apple/applearchive/) med inställningar som används för sammansatta poster. |
| AppleArchive(source_stream, load_options) | Initierar en ny instans av klassen [AppleArchive](/zip/python-net/aspose.zip.apple/applearchive/) och sammansätter en postlista som kan extraheras från arkivet. |
| AppleArchive(path, load_options) | Initierar en ny instans av klassen [AppleArchive](/zip/python-net/aspose.zip.apple/applearchive/) och sammansätter en postlista som kan extraheras från arkivet. |
## Egenskaper
| Namn | Beskrivning |
| :- | :- |
| poster | Hämtar poster som utgör arkivet. |
| is_solid | Hämtar ett värde som indikerar om arkivet använder solid kompression.<br/>            I solid läge komprimeras all postdata som en enda ström och<br/>            individuell postextraktion är inte tillgänglig. Använd |
| new_entry_settings | Hämtar inställningar som används för nyss sammansatta poster. |
| file_entries | Hämtar poster av typen [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) som utgör arkivet. |
| format | Hämtar arkivformatet. |
## Metoder
| Namn | Beskrivning |
| :- | :- |
| create_entry(name, path, open_immediately) | Skapar en enda post i arkivet. |
| create_entry(name, source) | Skapar en enda post i arkivet. |
| create_entry(name, file_info, open_immediately) | Skapar en enda post i arkivet. |
| save(output) | Sparar arkivet till den angivna strömmen. |
| save(destination_file_name) | Sparar arkivet till den angivna destinationsfilen. |
| create_entries(directory, include_root_directory) | Lägger till alla filer och kataloger rekursivt i den angivna katalogen i arkivet. |
| extract_to_directory(destination_directory) | Extraherar alla filer i arkivet till den angivna katalogen. |

### Se även

* namespace [aspose.zip.apple](/zip/python-net/aspose.zip.apple/)
* assembly [Aspose.Zip](/zip/python-net/)

