---
title: "IsoArchive"
second_title: "Aspose.Zip för Python via .NET API-referens"
description: 
type: docs
weight: 30
url: /sv/python-net/aspose.zip.iso/isoarchive/
---

## IsoArchive class

Representerar ett ISO-arkiv (ISO 9660).

Typen IsoArchive exponerar följande medlemmar:
## Konstruktörer
| Namn | Beskrivning |
| :- | :- |
| IsoArchive() | Initierar en ny instans av klassen [IsoArchive](/zip/python-net/aspose.zip.iso/isoarchive/) och skapar ett tomt ISO‑arkiv<br/>             för att lägga till nya filer och kataloger. |
| IsoArchive(source_stream, load_options) | Initierar en ny instans av klassen [IsoArchive](/zip/python-net/aspose.zip.iso/isoarchive/) och sammanställer en postlista som kan extraheras från arkivet. |
| IsoArchive(path, load_options) | Initierar en ny instans av klassen [IsoArchive](/zip/python-net/aspose.zip.iso/isoarchive/) och sammanställer en postlista som kan extraheras från arkivet. |
## Egenskaper
| Namn | Beskrivning |
| :- | :- |
| entries | Hämtar poster av typen [IsoEntry](/zip/python-net/aspose.zip.iso/isoentry/) som utgör arkivet. |
| file_entries | Hämtar poster av typen [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) som utgör arkivet. |
| format | Hämtar arkivformatet. |
## Metoder
| Namn | Beskrivning |
| :- | :- |
| create_entry(name, file_path) | Lägger till en fil i ISO‑avbilden. |
| create_entry(name, source) | Lägger till en fil i ISO‑avbilden. |
| create_entry(name) | Lägger till en fil i ISO‑avbilden. |
| save(path, save_options) | Sparar ISO‑avbilden till den angivna sökvägen. |
| save(stream, save_options) | Sparar ISO‑avbilden till den angivna strömmen. |
| create_directory(name) | Lägger till en katalog i ISO‑avbilden. |
| extract_to_directory(destination_directory) | Extraherar alla poster till den angivna katalogen. |

### Se även

* namespace [aspose.zip.iso](/zip/python-net/aspose.zip.iso/)
* assembly [Aspose.Zip](/zip/python-net/)

