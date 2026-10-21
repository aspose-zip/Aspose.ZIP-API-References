---
title: "TarArchive"
second_title: "Aspose.Zip för Python via .NET API-referens"
description: 
type: docs
weight: 10
url: /sv/python-net/aspose.zip.tar/tararchive/
---

## TarArchive class

Denna klass representerar en tar-arkivfil. Använd den för att skapa, extrahera eller uppdatera tar-arkiv.

Typen TarArchive exponerar följande medlemmar:
## Konstruktörer
| Namn | Beskrivning |
| :- | :- |
| TarArchive() | Initierar en ny instans av klassen [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/). |
| TarArchive(source_stream) | Initierar en ny instans av klassen [Archive](/zip/python-net/aspose.zip/archive/) och samlar en postlista som kan extraheras från arkivet. |
| TarArchive(path) | Initierar en ny instans av klassen [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) och skapar en postlista som kan extraheras från arkivet. |
## Egenskaper
| Namn | Beskrivning |
| :- | :- |
| entries | Hämtar poster av typen [TarEntry](/zip/python-net/aspose.zip.tar/tarentry/) som utgör arkivet. |
| file_entries | Hämtar poster av typen [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) som utgör arkivet. |
| format | Hämtar arkivformatet. |
## Metoder
| Namn | Beskrivning |
| :- | :- |
| create_entry(name, source, file_info) | Skapa en enskild post i arkivet. |
| create_entry(name, file_info, open_immediately) | Skapa en enskild post i arkivet. |
| create_entry(name, path, open_immediately) | Skapa en enskild post i arkivet. |
| create_entries(directory, include_root_directory) | Lägger till alla filer och kataloger rekursivt i den angivna katalogen i arkivet. |
| create_entries(source_directory, include_root_directory) | Lägger till alla filer och kataloger rekursivt i den angivna katalogen i arkivet. |
| delete_entry(entry) | Tar bort den första förekomsten av en specifik post från postlistan. |
| delete_entry(entry_index) |  |
| save(output, format) |  |
| save(destination_file_name, format) |  |
| save_gzipped(output, format) |  |
| save_gzipped(path, format) |  |
| save_zstandard(output, format) |  |
| save_zstandard(path, format) |  |
| save_lzipped(output, format) |  |
| save_lzipped(path, format) |  |
| save_lzma_compressed(output, format) |  |
| save_lzma_compressed(path, format) |  |
| save_lz4_compressed(output, format) |  |
| save_lz4_compressed(path, format) |  |
| save_xz_compressed(output, format, settings) |  |
| save_xz_compressed(path, format, settings) |  |
| save_z_compressed(output, format) |  |
| save_z_compressed(path, format) |  |
| from_g_zip(source) | Extraherar det medföljande gzip‑arkivet och skapar [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) från de extraherade data. |
| from_g_zip(path) | Extraherar det medföljande gzip‑arkivet och skapar [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) från de extraherade data. |
| from_zstandard(source) | Extraherar det medföljande Zstandard‑arkivet och skapar [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) från de extraherade data. |
| from_zstandard(path) | Extraherar det medföljande Zstandard‑arkivet och skapar [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) från de extraherade data. |
| from_l_zip(source) | Extraherar det medföljande lzip‑arkivet och skapar [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) från de extraherade data. |
| from_l_zip(path) | Extraherar det medföljande lzip‑arkivet och skapar [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) från de extraherade data. |
| from_lzma(source) | Extraherar det medföljande LZMA‑arkivet och skapar [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) från de extraherade data. |
| from_lzma(path) | Extraherar det medföljande LZMA‑arkivet och skapar [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) från de extraherade data. |
| from_lz4(path) | Extraherar det medföljande LZ4‑arkivet och skapar [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) från de extraherade data. |
| from_lz4(source) | Extraherar det medföljande LZ4‑arkivet och skapar [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) från de extraherade data. |
| from_xz(source) | Extraherar det medföljande xz‑formatarkivet och skapar [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) från de extraherade data. |
| from_xz(path) | Extraherar det medföljande xz‑formatarkivet och skapar [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) från de extraherade data. |
| from_z(source) | Extraherar det medföljande Zstandard‑arkivet och skapar [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) från de extraherade data. |
| from_z(path) | Extraherar det medföljande Zstandard‑arkivet och skapar [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) från de extraherade data. |
| extract_to_directory(destination_directory) | Extraherar alla filer i arkivet till den angivna katalogen. |

### Se även

* namespace [aspose.zip.tar](/zip/python-net/aspose.zip.tar/)
* assembly [Aspose.Zip](/zip/python-net/)

