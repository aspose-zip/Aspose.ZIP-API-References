---
title: "SharArchive"
second_title: "Aspose.Zip для Python через .NET Справочник API"
description: 
type: docs
weight: 10
url: /ru/python-net/aspose.zip.shar/shararchive/
---

## SharArchive class

Этот класс представляет файл архива shar.

Тип SharArchive раскрывает следующие члены:
## Конструкторы
| Имя | Описание |
| :- | :- |
| SharArchive() | Инициализирует новый экземпляр класса [SharArchive](/zip/python-net/aspose.zip.shar/shararchive/). |
| SharArchive(path) | Инициализирует новый экземпляр класса [SharArchive](/zip/python-net/aspose.zip.shar/shararchive/) для распаковки. |
## Свойства
| Имя | Описание |
| :- | :- |
| entries | Получает элементы типа [SharEntry](/zip/python-net/aspose.zip.shar/sharentry/), составляющие архив. |
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
| save(destination_file_name) | Сохраняет архив в указанный файл назначения. |
| save(output) | Сохраняет архив в предоставленный поток. |

### См. также

* namespace [aspose.zip.shar](/zip/python-net/aspose.zip.shar/)
* assembly [Aspose.Zip](/zip/python-net/)

