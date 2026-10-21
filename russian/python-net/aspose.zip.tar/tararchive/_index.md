---
title: "TarArchive"
second_title: "Aspose.Zip для Python через .NET Справочник API"
description: 
type: docs
weight: 10
url: /ru/python-net/aspose.zip.tar/tararchive/
---

## TarArchive class

Этот класс представляет файл архива tar. Используйте его для создания, извлечения или обновления архивов tar.

Тип TarArchive раскрывает следующие члены:
## Конструкторы
| Имя | Описание |
| :- | :- |
| TarArchive() | Инициализирует новый экземпляр класса [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/). |
| TarArchive(source_stream) | Инициализирует новый экземпляр класса [Archive](/zip/python-net/aspose.zip/archive/) и формирует список записей, которые можно извлечь из архива. |
| TarArchive(path) | Инициализирует новый экземпляр класса [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) и формирует список записей, которые можно извлечь из архива. |
## Свойства
| Имя | Описание |
| :- | :- |
| entries | Получает записи типа [TarEntry](/zip/python-net/aspose.zip.tar/tarentry/), составляющие архив. |
| file_entries | Получает записи типа [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/), составляющие архив. |
| format | Возвращает формат архива. |
## Методы
| Имя | Описание |
| :- | :- |
| create_entry(name, source, file_info) | Создаёт одну запись внутри архива. |
| create_entry(name, file_info, open_immediately) | Создаёт одну запись внутри архива. |
| create_entry(name, path, open_immediately) | Создаёт одну запись внутри архива. |
| create_entries(directory, include_root_directory) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| create_entries(source_directory, include_root_directory) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| delete_entry(entry) | Удаляет первое вхождение конкретной записи из списка записей. |
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
| from_g_zip(source) | Извлекает предоставленный gzip-архив и создает [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) из извлечённых данных. |
| from_g_zip(path) | Извлекает предоставленный gzip-архив и создает [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) из извлечённых данных. |
| from_zstandard(source) | Извлекает предоставленный архив Zstandard и создает [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) из извлечённых данных. |
| from_zstandard(path) | Извлекает предоставленный архив Zstandard и создает [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) из извлечённых данных. |
| from_l_zip(source) | Извлекает предоставленный lzip-архив и создает [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) из извлечённых данных. |
| from_l_zip(path) | Извлекает предоставленный lzip-архив и создает [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) из извлечённых данных. |
| from_lzma(source) | Извлекает предоставленный LZMA-архив и создает [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) из извлечённых данных. |
| from_lzma(path) | Извлекает предоставленный LZMA-архив и создает [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) из извлечённых данных. |
| from_lz4(path) | Извлекает предоставленный LZ4-архив и создает [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) из извлечённых данных. |
| from_lz4(source) | Извлекает предоставленный LZ4-архив и создает [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) из извлечённых данных. |
| from_xz(source) | Извлекает предоставленный архив в формате xz и создает [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) из извлечённых данных. |
| from_xz(path) | Извлекает предоставленный архив в формате xz и создает [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) из извлечённых данных. |
| from_z(source) | Извлекает предоставленный архив Zstandard и создает [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) из извлечённых данных. |
| from_z(path) | Извлекает предоставленный архив Zstandard и создает [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) из извлечённых данных. |
| extract_to_directory(destination_directory) | Извлекает все файлы из архива в указанный каталог. |

### См. также

* namespace [aspose.zip.tar](/zip/python-net/aspose.zip.tar/)
* assembly [Aspose.Zip](/zip/python-net/)

