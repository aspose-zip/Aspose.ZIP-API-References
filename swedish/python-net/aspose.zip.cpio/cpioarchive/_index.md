---
title: "CpioArchive"
second_title: "Aspose.Zip för Python via .NET API-referens"
description: 
type: docs
weight: 10
url: /sv/python-net/aspose.zip.cpio/cpioarchive/
---

## CpioArchive class

Denna klass representerar en cpio-arkivfil.

CpioArchive-typen exponerar följande medlemmar:
## Konstruktörer
| Namn | Beskrivning |
| :- | :- |
| CpioArchive() | Initierar en ny instans av klassen [CpioArchive](/zip/python-net/aspose.zip.cpio/cpioarchive/). |
| CpioArchive(source_stream) | Initierar en ny instans av klassen [CpioArchive](/zip/python-net/aspose.zip.cpio/cpioarchive/) och skapar en postlista som kan extraheras från arkivet. |
| CpioArchive(path) | Initierar en ny instans av klassen [CpioArchive](/zip/python-net/aspose.zip.cpio/cpioarchive/) och skapar en postlista som kan extraheras från arkivet. |
## Egenskaper
| Namn | Beskrivning |
| :- | :- |
| entries | Hämtar poster av typen [CpioEntry](/zip/python-net/aspose.zip.cpio/cpioentry/) som utgör arkivet. |
| file_entries | Hämtar poster av typen [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) som utgör arkivet. |
| format | Hämtar arkivformatet. |
## Metoder
| Namn | Beskrivning |
| :- | :- |
| create_entries(source_directory, include_root_directory) | Lägger till alla filer och kataloger rekursivt i den angivna katalogen i arkivet. |
| create_entries(directory, include_root_directory) | Lägger till alla filer och kataloger rekursivt i den angivna katalogen i arkivet. |
| create_entry(name, file_info, open_immediately) | Skapa en enskild post i arkivet. |
| create_entry(name, source_path, open_immediately) | Skapa en enskild post i arkivet. |
| create_entry(name, source) | Skapa en enskild post i arkivet. |
| delete_entry(entry) | Tar bort den första förekomsten av en specifik post från postlistan. |
| delete_entry(entry_index) |  |
| save(destination_file_name, cpio_format) | Sparar arkivet till den angivna destinationsfilen. |
| save(output, cpio_format) | Sparar arkivet till den angivna strömmen. |
| save_gzipped(output, cpio_format) | Sparar arkivet till strömmen med gzip-komprimering. |
| save_gzipped(path, cpio_format) | Sparar arkivet till filen via sökväg med gzip-komprimering. |
| save_lzipped(output, cpio_format) | Sparar arkivet till strömmen med lzip-komprimering. |
| save_lzipped(path, cpio_format) | Sparar arkivet till filen via sökväg med lzip-komprimering. |
| save_lzma_compressed(output, cpio_format) | Sparar arkivet till strömmen med LZMA-komprimering. |
| save_lzma_compressed(path, cpio_format) | Sparar arkivet till filen via sökväg med lzma-komprimering. |
| save_xz_compressed(output, cpio_format, settings) | Sparar arkivet till strömmen med xz-komprimering. |
| save_xz_compressed(path, cpio_format, settings) | Sparar arkivet till sökvägen via sökväg med xz-komprimering. |
| save_z_compressed(output, cpio_format) | Sparar arkivet till strömmen med Z-komprimering. |
| save_z_compressed(path, cpio_format) | Sparar arkivet till sökvägen med Z-komprimering. |
| save_zstandard(output, cpio_format) | Sparar arkivet till strömmen med Zstandard-komprimering. |
| save_zstandard(path, cpio_format) | Sparar arkivet till filen via sökväg med Zstandard-komprimering. |
| extract_to_directory(destination_directory) | Extraherar alla filer i arkivet till den angivna katalogen. |

### Se även

* namespace [aspose.zip.cpio](/zip/python-net/aspose.zip.cpio/)
* assembly [Aspose.Zip](/zip/python-net/)

