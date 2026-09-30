---
title: "AppleArchive"
second_title: "Aspose.Zip для Python через .NET Справочник API"
description: 
type: docs
weight: 10
url: /ru/python-net/aspose.zip.apple/applearchive/
---

## AppleArchive class

Этот класс представляет файл Apple Archive (.aar). Используйте его для создания файлов Apple Archive.

Тип AppleArchive раскрывает следующие члены:
## Конструкторы
| Имя | Описание |
| :- | :- |
| AppleArchive(new_entry_settings) | Инициализирует новый экземпляр класса [AppleArchive](/zip/python-net/aspose.zip.apple/applearchive/) с настройками, используемыми для составных записей. |
| AppleArchive(source_stream, load_options) | Инициализирует новый экземпляр класса [AppleArchive](/zip/python-net/aspose.zip.apple/applearchive/) и формирует список записей, который может быть извлечён из архива. |
| AppleArchive(path, load_options) | Инициализирует новый экземпляр класса [AppleArchive](/zip/python-net/aspose.zip.apple/applearchive/) и формирует список записей, который может быть извлечён из архива. |
## Свойства
| Имя | Описание |
| :- | :- |
| entries | Получает записи, составляющие архив. |
| is_solid | Получает значение, указывающее, использует ли архив сплошное сжатие.<br/>            В сплошном режиме все данные записей сжаты в один поток и<br/>            отдельное извлечение записей недоступно. Используйте |
| new_entry_settings | Получает параметры, используемые для вновь созданных записей. |
| file_entries | Получает записи типа [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/), составляющие архив. |
| format | Возвращает формат архива. |
## Методы
| Имя | Описание |
| :- | :- |
| create_entry(name, path, open_immediately) | Создаёт одну запись в архиве. |
| create_entry(name, source) | Создаёт одну запись в архиве. |
| create_entry(name, file_info, open_immediately) | Создаёт одну запись в архиве. |
| save(output) | Сохраняет архив в предоставленный поток. |
| save(destination_file_name) | Сохраняет архив в указанный файл назначения. |
| create_entries(directory, include_root_directory) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| extract_to_directory(destination_directory) | Извлекает все файлы из архива в указанный каталог. |

### См. также

* namespace [aspose.zip.apple](/zip/python-net/aspose.zip.apple/)
* assembly [Aspose.Zip](/zip/python-net/)

