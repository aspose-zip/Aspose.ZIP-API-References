---
title: "ZArchive"
second_title: "Aspose.Zip для Python через .NET Справочник API"
description: 
type: docs
weight: 10
url: /ru/python-net/aspose.zip.z/zarchive/
---

## ZArchive class

Этот класс представляет файл архива Z (compress). Используйте его для создания или извлечения архивов Z.

Тип ZArchive раскрывает следующие члены:
## Конструкторы
| Имя | Описание |
| :- | :- |
| ZArchive() | Инициализирует новый экземпляр класса [ZArchive](/zip/python-net/aspose.zip.z/zarchive/) подготовленного для сжатия. |
| ZArchive(source, load_options) | Инициализирует новый экземпляр класса [ZArchive](/zip/python-net/aspose.zip.z/zarchive/) подготовленного для распаковки. |
| ZArchive(path, load_options) | Инициализирует новый экземпляр класса [ZArchive](/zip/python-net/aspose.zip.z/zarchive/) подготовленного для распаковки. |
## Свойства
| Имя | Описание |
| :- | :- |
| file_entries | Получает записи типа [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/), составляющие архив. |
| format | Возвращает формат архива. |
| name | Получает имя записи. |
| length | Получает длину записи в байтах. |
## Методы
| Имя | Описание |
| :- | :- |
| extract(destination) | Извлекает архив Z в поток. |
| extract(file_info) | Извлекает архив Z в файл. |
| extract(path) | Извлекает архив Z в файл по пути. |
| save(output, settings) | Сохраняет архив xz в указанный поток. |
| save(destination_file_name, settings) | Сохраняет архив Z в указанный файл назначения. |
| set_source(source) | Устанавливает содержимое, которое будет сжато в архиве. |
| set_source(file_info) | Устанавливает содержимое, которое будет сжато в архиве. |
| set_source(source_path) | Устанавливает содержимое, которое будет сжато в архиве. |
| extract_to_directory(destination_directory) | Извлекает содержимое архива в предоставленный каталог. |

### См. также

* namespace [aspose.zip.z](/zip/python-net/aspose.zip.z/)
* assembly [Aspose.Zip](/zip/python-net/)

