---
title: "IsoArchive"
second_title: "Aspose.Zip для Python через .NET Справочник API"
description: 
type: docs
weight: 30
url: /ru/python-net/aspose.zip.iso/isoarchive/
---

## IsoArchive class

Представляет ISO‑архив (ISO 9660).

Тип IsoArchive раскрывает следующие члены:
## Конструкторы
| Имя | Описание |
| :- | :- |
| IsoArchive() | Инициализирует новый экземпляр класса [IsoArchive](/zip/python-net/aspose.zip.iso/isoarchive/) и создает пустой ISO‑архив<br/>             для добавления новых файлов и каталогов. |
| IsoArchive(source_stream, load_options) | Инициализирует новый экземпляр класса [IsoArchive](/zip/python-net/aspose.zip.iso/isoarchive/) и формирует список записей, которые можно извлечь из архива. |
| IsoArchive(path, load_options) | Инициализирует новый экземпляр класса [IsoArchive](/zip/python-net/aspose.zip.iso/isoarchive/) и формирует список записей, которые можно извлечь из архива. |
## Свойства
| Имя | Описание |
| :- | :- |
| entries | Получает записи типа [IsoEntry](/zip/python-net/aspose.zip.iso/isoentry/), составляющие архив. |
| file_entries | Получает записи типа [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/), составляющие архив. |
| format | Возвращает формат архива. |
## Методы
| Имя | Описание |
| :- | :- |
| create_entry(name, file_path) | Добавляет файл в ISO‑образ. |
| create_entry(name, source) | Добавляет файл в ISO‑образ. |
| create_entry(name) | Добавляет файл в ISO‑образ. |
| save(path, save_options) | Сохраняет ISO‑образ по указанному пути. |
| save(stream, save_options) | Сохраняет ISO‑образ в указанный поток. |
| create_directory(name) | Добавляет каталог в ISO‑образ. |
| extract_to_directory(destination_directory) | Извлекает все записи в указанный каталог. |

### См. также

* namespace [aspose.zip.iso](/zip/python-net/aspose.zip.iso/)
* assembly [Aspose.Zip](/zip/python-net/)

