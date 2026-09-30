---
title: "Archive"
second_title: "Aspose.Zip для Python через .NET Справочник API"
description: 
type: docs
weight: 10
url: /ru/python-net/aspose.zip/archive/
---

## Archive class

Этот класс представляет файл zip‑архива. Используйте его для создания, извлечения или обновления zip‑архивов.

Тип Archive раскрывает следующие члены:
## Конструкторы
| Имя | Описание |
| :- | :- |
| Archive(new_entry_settings) | Инициализирует новый экземпляр класса [Archive](/zip/python-net/aspose.zip/archive/) с необязательными настройками для его записей. |
| Archive(source_stream, load_options, new_entry_settings) | Инициализирует новый экземпляр класса [Archive](/zip/python-net/aspose.zip/archive/) и формирует список записей, которые можно извлечь из архива. |
| Archive(path, load_options, new_entry_settings) | Инициализирует новый экземпляр класса [Archive](/zip/python-net/aspose.zip/archive/) и формирует список записей, которые можно извлечь из архива. |
| Archive(main_segment, segments_in_order, load_options) | Инициализирует новый экземпляр класса [Archive](/zip/python-net/aspose.zip/archive/) из многотомного ZIP-архива и формирует список записей, которые можно извлечь из архива. |
## Свойства
| Имя | Описание |
| :- | :- |
| new_entry_settings | Параметры сжатия и шифрования, используемые для недавно добавленных элементов [ArchiveEntry](/zip/python-net/aspose.zip/archiveentry/). |
| comment | Получает комментарий для всего архива. |
| entries | Получает записи типа [ArchiveEntry](/zip/python-net/aspose.zip/archiveentry/), составляющие архив. |
| file_entries | Получает записи типа [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/), составляющие архив. |
| format | Возвращает формат архива. |
## Методы
| Имя | Описание |
| :- | :- |
| create_entry(name, path, open_immediately, new_entry_settings) | Создаёт одну запись внутри архива. |
| create_entry(name, source, new_entry_settings) | Создаёт одну запись внутри архива. |
| create_entry(name, file_info, open_immediately, new_entry_settings) | Создаёт одну запись внутри архива. |
| create_entry(name, source, new_entry_settings, file_info) | Создаёт одну запись внутри архива. |
| create_entries(directory, include_root_directory) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| create_entries(source_directory, include_root_directory) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| delete_entry(entry) | Удаляет первое вхождение указанной записи из списка записей. |
| delete_entry(entry_index) |  |
| save(output_stream, save_options) | Сохраняет архив в предоставленный поток. |
| save(destination_file_name, save_options) | Сохраняет архив в указанный файл назначения. |
| save_split(destination_directory, options) | Сохраняет многотомный архив в указанный каталог назначения. |
| extract_to_directory(destination_directory) | Извлекает все файлы из архива в указанный каталог. |

### См. также

* namespace [aspose.zip](/zip/python-net/aspose.zip/)
* assembly [Aspose.Zip](/zip/python-net/)

