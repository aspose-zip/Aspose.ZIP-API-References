---
title: "CpioArchive"
second_title: "Aspose.Zip для Python через .NET Справочник API"
description: 
type: docs
weight: 10
url: /ru/python-net/aspose.zip.cpio/cpioarchive/
---

## CpioArchive class

Этот класс представляет файл архива cpio.

Тип CpioArchive раскрывает следующие члены:
## Конструкторы
| Имя | Описание |
| :- | :- |
| CpioArchive() | Инициализирует новый экземпляр класса [CpioArchive](/zip/python-net/aspose.zip.cpio/cpioarchive/). |
| CpioArchive(source_stream) | Инициализирует новый экземпляр класса [CpioArchive](/zip/python-net/aspose.zip.cpio/cpioarchive/) и формирует список записей, которые можно извлечь из архива. |
| CpioArchive(path) | Инициализирует новый экземпляр класса [CpioArchive](/zip/python-net/aspose.zip.cpio/cpioarchive/) и формирует список записей, которые можно извлечь из архива. |
## Свойства
| Имя | Описание |
| :- | :- |
| entries | Получает записи типа [CpioEntry](/zip/python-net/aspose.zip.cpio/cpioentry/), составляющие архив. |
| file_entries | Получает записи типа [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/), составляющие архив. |
| format | Возвращает формат архива. |
## Методы
| Имя | Описание |
| :- | :- |
| create_entries(source_directory, include_root_directory) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| create_entries(directory, include_root_directory) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| create_entry(name, file_info, open_immediately) | Создаёт одну запись внутри архива. |
| create_entry(name, source_path, open_immediately) | Создаёт одну запись внутри архива. |
| create_entry(name, source) | Создаёт одну запись внутри архива. |
| delete_entry(entry) | Удаляет первое вхождение конкретной записи из списка записей. |
| delete_entry(entry_index) |  |
| save(destination_file_name, cpio_format) | Сохраняет архив в указанный файл назначения. |
| save(output, cpio_format) | Сохраняет архив в предоставленный поток. |
| save_gzipped(output, cpio_format) | Сохраняет архив в поток с gzip‑сжатием. |
| save_gzipped(path, cpio_format) | Сохраняет архив в файл по пути с gzip‑сжатием. |
| save_lzipped(output, cpio_format) | Сохраняет архив в поток с lzip‑сжатием. |
| save_lzipped(path, cpio_format) | Сохраняет архив в файл по пути с lzip‑сжатием. |
| save_lzma_compressed(output, cpio_format) | Сохраняет архив в поток с LZMA‑сжатием. |
| save_lzma_compressed(path, cpio_format) | Сохраняет архив в файл по пути с lzma‑сжатием. |
| save_xz_compressed(output, cpio_format, settings) | Сохраняет архив в поток с xz‑сжатием. |
| save_xz_compressed(path, cpio_format, settings) | Сохраняет архив по пути с xz‑сжатием. |
| save_z_compressed(output, cpio_format) | Сохраняет архив в поток с Z‑сжатием. |
| save_z_compressed(path, cpio_format) | Сохраняет архив по указанному пути с Z‑сжатием. |
| save_zstandard(output, cpio_format) | Сохраняет архив в поток с Zstandard‑сжатием. |
| save_zstandard(path, cpio_format) | Сохраняет архив в файл по пути с Zstandard‑сжатием. |
| extract_to_directory(destination_directory) | Извлекает все файлы из архива в указанный каталог. |

### См. также

* namespace [aspose.zip.cpio](/zip/python-net/aspose.zip.cpio/)
* assembly [Aspose.Zip](/zip/python-net/)

