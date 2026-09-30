---
title: "XarArchive"
second_title: "Aspose.Zip для Python через .NET Справочник API"
description: 
type: docs
weight: 40
url: /ru/python-net/aspose.zip.xar/xararchive/
---

## XarArchive class

Этот класс представляет файл архива xar.

Тип XarArchive раскрывает следующие члены:
## Конструкторы
| Имя | Описание |
| :- | :- |
| XarArchive(default_compression_settings) | Инициализирует новый экземпляр класса [XarArchive](/zip/python-net/aspose.zip.xar/xararchive/). |
| XarArchive(source_stream, load_options) | Инициализирует новый экземпляр класса [XarArchive](/zip/python-net/aspose.zip.xar/xararchive/) и формирует список записей, которые можно извлечь из архива. |
| XarArchive(path, load_options) | Инициализирует новый экземпляр класса [XarArchive](/zip/python-net/aspose.zip.xar/xararchive/) и формирует список записей, которые можно извлечь из архива. |
## Свойства
| Имя | Описание |
| :- | :- |
| entries | Получает записи типа [XarEntry](/zip/python-net/aspose.zip.xar/xarentry/), составляющие архив. |
| file_entries | Получает записи типа [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/), составляющие архив. |
| format | Возвращает формат архива. |
## Методы
| Имя | Описание |
| :- | :- |
| create_entries(source_directory, include_root_directory, compression_settings) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| create_entries(directory, include_root_directory, compression_settings) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| create_entry(name, file_info, open_immediately, compression_settings) | Создаёт одну запись внутри архива. |
| create_entry(name, source_path, open_immediately, compression_settings) | Создаёт одну запись внутри архива. |
| create_entry(name, source, compression_settings) | Создаёт одну запись внутри архива. |
| save(destination_file_name, save_options) | Сохраняет архив в указанный файл назначения. |
| save(output, save_options) | Сохраняет архив в предоставленный поток. |
| extract_to_directory(destination_directory) | Извлекает все файлы из архива в указанный каталог. |
| delete_entry(entry) | Удаляет первое вхождение конкретной записи из списка записей. |

### См. также

* namespace [aspose.zip.xar](/zip/python-net/aspose.zip.xar/)
* assembly [Aspose.Zip](/zip/python-net/)

