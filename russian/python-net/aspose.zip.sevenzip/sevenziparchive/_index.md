---
title: "SevenZipArchive"
second_title: "Aspose.Zip для Python через .NET Справочник API"
description: 
type: docs
weight: 10
url: /ru/python-net/aspose.zip.sevenzip/sevenziparchive/
---

## SevenZipArchive class

Этот класс представляет файл 7z‑архива. Используйте его для создания и извлечения 7z‑архивов.

Тип SevenZipArchive раскрывает следующие члены:
## Конструкторы
| Имя | Описание |
| :- | :- |
| SevenZipArchive(new_entry_settings) | Инициализирует новый экземпляр класса [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) с необязательными настройками для его элементов. |
| SevenZipArchive(source_stream, password) | Инициализирует новый экземпляр класса [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) и формирует список записей, которые можно извлечь из архива. |
| SevenZipArchive(path, password) | Инициализирует новый экземпляр класса [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) и формирует список записей, которые можно извлечь из архива. |
| SevenZipArchive(source_stream, options) | Инициализирует новый экземпляр класса [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) и формирует список записей, которые можно извлечь из архива. |
| SevenZipArchive(path, options) | Инициализирует новый экземпляр класса [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) и формирует список записей, которые можно извлечь из архива. |
| SevenZipArchive(parts, password) | Инициализирует новый экземпляр класса [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) из многотомного 7z-архива и формирует список записей, которые можно извлечь из архива. |
## Свойства
| Имя | Описание |
| :- | :- |
| new_entry_settings | Настройки сжатия и шифрования, используемые для недавно добавленных элементов [SevenZipArchiveEntry](/zip/python-net/aspose.zip.sevenzip/sevenziparchiveentry/). |
| entries | Получает записи типа [SevenZipArchiveEntry](/zip/python-net/aspose.zip.sevenzip/sevenziparchiveentry/), составляющие архив. |
| file_entries | Получает записи типа [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/), составляющие архив. |
| format | Возвращает формат архива. |
## Методы
| Имя | Описание |
| :- | :- |
| create_entry(name, file_info, open_immediately, new_entry_settings) | Создаёт одну запись внутри архива. |
| create_entry(name, source, new_entry_settings, file_info) | Создаёт одну запись внутри архива. |
| create_entry(name, source, new_entry_settings) | Создаёт одну запись внутри архива. |
| create_entry(name, path, open_immediately, new_entry_settings) | Создаёт одну запись внутри архива. |
| create_entries(directory, include_root_directory) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| create_entries(source_directory, include_root_directory) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| save(output, save_options) | Сохраняет 7z-архив в указанный поток. |
| save(destination_file_name, save_options) | Сохраняет архив в указанный файл назначения. |
| extract_to_directory(destination_directory, password) | Извлекает все файлы из архива в указанный каталог. |
| extract_to_directory(destination_directory) | Извлекает все файлы из архива в указанный каталог. |
| save_split(destination_directory, options) | Сохраняет многотомный архив в указанный каталог назначения. |

### См. также

* namespace [aspose.zip.sevenzip](/zip/python-net/aspose.zip.sevenzip/)
* assembly [Aspose.Zip](/zip/python-net/)

