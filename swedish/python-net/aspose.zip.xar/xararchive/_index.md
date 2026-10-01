---
title: "XarArchive"
second_title: "Aspose.Zip för Python via .NET API-referens"
description: 
type: docs
weight: 40
url: /sv/python-net/aspose.zip.xar/xararchive/
---

## XarArchive class

Denna klass representerar en xar-arkivfil.

XarArchive-typen exponerar följande medlemmar:
## Konstruktörer
| Namn | Beskrivning |
| :- | :- |
| XarArchive(default_compression_settings) | Initierar en ny instans av klassen [XarArchive](/zip/python-net/aspose.zip.xar/xararchive/). |
| XarArchive(source_stream, load_options) | Initierar en ny instans av klassen [XarArchive](/zip/python-net/aspose.zip.xar/xararchive/) och skapar en postlista som kan extraheras från arkivet. |
| XarArchive(path, load_options) | Initierar en ny instans av klassen [XarArchive](/zip/python-net/aspose.zip.xar/xararchive/) och skapar en postlista som kan extraheras från arkivet. |
## Egenskaper
| Namn | Beskrivning |
| :- | :- |
| entries | Hämtar poster av typen [XarEntry](/zip/python-net/aspose.zip.xar/xarentry/) som utgör arkivet. |
| file_entries | Hämtar poster av typen [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) som utgör arkivet. |
| format | Hämtar arkivformatet. |
## Metoder
| Namn | Beskrivning |
| :- | :- |
| create_entries(source_directory, include_root_directory, compression_settings) | Lägger till alla filer och kataloger rekursivt i den angivna katalogen i arkivet. |
| create_entries(directory, include_root_directory, compression_settings) | Lägger till alla filer och kataloger rekursivt i den angivna katalogen i arkivet. |
| create_entry(name, file_info, open_immediately, compression_settings) | Skapa en enskild post i arkivet. |
| create_entry(name, source_path, open_immediately, compression_settings) | Skapa en enskild post i arkivet. |
| create_entry(name, source, compression_settings) | Skapa en enskild post i arkivet. |
| save(destination_file_name, save_options) | Sparar arkivet till den angivna destinationsfilen. |
| save(output, save_options) | Sparar arkivet till den angivna strömmen. |
| extract_to_directory(destination_directory) | Extraherar alla filer i arkivet till den angivna katalogen. |
| delete_entry(entry) | Tar bort den första förekomsten av en specifik post från postlistan. |

### Se även

* namespace [aspose.zip.xar](/zip/python-net/aspose.zip.xar/)
* assembly [Aspose.Zip](/zip/python-net/)

