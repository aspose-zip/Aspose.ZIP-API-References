---
title: "CabArchive"
second_title: "Aspose.Zip для Python через .NET Справочник API"
description: 
type: docs
weight: 10
url: /ru/python-net/aspose.zip.cab/cabarchive/
---

## CabArchive class

Этот класс представляет файл архива CAB.

Тип CabArchive раскрывает следующие члены:
## Конструкторы
| Имя | Описание |
| :- | :- |
| CabArchive(settings) | Инициализирует новый экземпляр класса [CabArchive](/zip/python-net/aspose.zip.cab/cabarchive/) подготовленного для сжатия. |
| CabArchive(source_stream, load_options) | Инициализирует новый экземпляр класса [CabArchive](/zip/python-net/aspose.zip.cab/cabarchive/) и формирует список записей, которые могут быть извлечены из архива. |
| CabArchive(path, load_options) | Инициализирует новый экземпляр класса [CabArchive](/zip/python-net/aspose.zip.cab/cabarchive/) и формирует список записей, которые могут быть извлечены из архива. |
## Свойства
| Имя | Описание |
| :- | :- |
| entries | Получает записи типа [CabEntry](/zip/python-net/aspose.zip.cab/cabentry/), составляющие архив. |
| file_entries | Получает записи типа [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/), составляющие архив. |
| format | Возвращает формат архива. |
## Методы
| Имя | Описание |
| :- | :- |
| create_entry(name, path, new_entry_settings) | Создаёт одну запись внутри архива. |
| create_entry(name, source, new_entry_settings) | Создаёт одну запись внутри архива. |
| create_entry(name, file_info, new_entry_settings) | Создаёт одну запись внутри архива. |
| create_entries(directory, include_root_directory) | Добавляет в архив все файлы, рекурсивно, из указанного каталога. |
| create_entries(source_directory, include_root_directory) | Добавляет в архив все файлы рекурсивно из указанного пути к каталогу. |
| save(output_stream, save_options) | Сохраняет архив в предоставленный поток. |
| save(destination_file_name, save_options) | Сохраняет архив в указанный файл назначения. |
| extract_to_directory(destination_directory) | Извлекает все файлы из архива в указанный каталог. |

### См. также

* namespace [aspose.zip.cab](/zip/python-net/aspose.zip.cab/)
* assembly [Aspose.Zip](/zip/python-net/)

