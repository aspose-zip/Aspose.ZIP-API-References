---
title: "SevenZipArchive"
second_title: "Aspose.Zip för Python via .NET API-referens"
description: 
type: docs
weight: 10
url: /sv/python-net/aspose.zip.sevenzip/sevenziparchive/
---

## SevenZipArchive class

Denna klass representerar en 7z-arkivfil. Använd den för att skapa och extrahera 7z-arkiv.

Typen SevenZipArchive exponerar följande medlemmar:
## Konstruktörer
| Namn | Beskrivning |
| :- | :- |
| SevenZipArchive(new_entry_settings) | Initierar en ny instans av klassen [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) med valfria inställningar för dess poster. |
| SevenZipArchive(source_stream, password) | Initierar en ny instans av klassen [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) och skapar en postlista som kan extraheras från arkivet. |
| SevenZipArchive(path, password) | Initierar en ny instans av klassen [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) och skapar en postlista som kan extraheras från arkivet. |
| SevenZipArchive(source_stream, options) | Initierar en ny instans av klassen [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) och skapar en postlista som kan extraheras från arkivet. |
| SevenZipArchive(path, options) | Initierar en ny instans av klassen [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) och skapar en postlista som kan extraheras från arkivet. |
| SevenZipArchive(parts, password) | Initierar en ny instans av klassen [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) från ett flervolym 7z-arkiv och skapar en postlista som kan extraheras från arkivet. |
## Egenskaper
| Namn | Beskrivning |
| :- | :- |
| new_entry_settings | Komprimerings- och krypteringsinställningar som används för nyss tillagda [SevenZipArchiveEntry](/zip/python-net/aspose.zip.sevenzip/sevenziparchiveentry/) objekt. |
| entries | Hämtar poster av typen [SevenZipArchiveEntry](/zip/python-net/aspose.zip.sevenzip/sevenziparchiveentry/) som utgör arkivet. |
| file_entries | Hämtar poster av typen [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) som utgör arkivet. |
| format | Hämtar arkivformatet. |
## Metoder
| Namn | Beskrivning |
| :- | :- |
| create_entry(name, file_info, open_immediately, new_entry_settings) | Skapa en enskild post i arkivet. |
| create_entry(name, source, new_entry_settings, file_info) | Skapa en enskild post i arkivet. |
| create_entry(name, source, new_entry_settings) | Skapa en enskild post i arkivet. |
| create_entry(name, path, open_immediately, new_entry_settings) | Skapa en enskild post i arkivet. |
| create_entries(directory, include_root_directory) | Lägger till alla filer och kataloger rekursivt i den angivna katalogen i arkivet. |
| create_entries(source_directory, include_root_directory) | Lägger till alla filer och kataloger rekursivt i den angivna katalogen i arkivet. |
| save(output, save_options) | Sparar 7z-arkivet till den angivna strömmen. |
| save(destination_file_name, save_options) | Sparar arkivet till den angivna destinationsfilen. |
| extract_to_directory(destination_directory, password) | Extraherar alla filer i arkivet till den angivna katalogen. |
| extract_to_directory(destination_directory) | Extraherar alla filer i arkivet till den angivna katalogen. |
| save_split(destination_directory, options) | Sparar flervolymigt arkiv till den angivna destinationskatalogen. |

### Se även

* namespace [aspose.zip.sevenzip](/zip/python-net/aspose.zip.sevenzip/)
* assembly [Aspose.Zip](/zip/python-net/)

