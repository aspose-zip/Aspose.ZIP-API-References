---
title: "ZstandardArchive"
second_title: "Aspose.Zip для Python через .NET Справочник API"
description: 
type: docs
weight: 10
url: /ru/python-net/aspose.zip.zstandard/zstandardarchive/
---

## ZstandardArchive class

Этот класс представляет файл архива Zstandard. Используйте его для создания архивов Zstandard.

Тип ZstandardArchive раскрывает следующие члены:
## Конструкторы
| Имя | Описание |
| :- | :- |
| ZstandardArchive() | Инициализирует новый экземпляр класса [ZstandardArchive](/zip/python-net/aspose.zip.zstandard/zstandardarchive/), подготовленного для сжатия. |
| ZstandardArchive(source_stream, options) | Инициализирует новый экземпляр класса [ZstandardArchive](/zip/python-net/aspose.zip.zstandard/zstandardarchive/), подготовленного для распаковки. |
| ZstandardArchive(path, options) | Инициализирует новый экземпляр класса [ZstandardArchive](/zip/python-net/aspose.zip.zstandard/zstandardarchive/). |
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
| extract(destination) | Извлекает архив в предоставленный поток. |
| extract(path) | Извлекает архив в файл по пути. |
| set_source(source) | Устанавливает содержимое, которое будет сжато в архиве. |
| set_source(file_info) | Устанавливает содержимое, которое будет сжато в архиве. |
| set_source(path) | Устанавливает содержимое, которое будет сжато в архиве. |
| save(output_stream, settings) | Сохраняет архив в предоставленный поток. |
| save(destination_file_name, settings) | Сохраняет архив в указанный файл назначения. |
| save(destination, settings) | Сохраняет архив в указанный файл назначения. |
| open() | Открывает архив для извлечения и предоставляет поток с содержимым архива. |
| extract_to_directory(destination_directory) | Извлекает содержимое архива в предоставленный каталог. |

### См. также

* namespace [aspose.zip.zstandard](/zip/python-net/aspose.zip.zstandard/)
* assembly [Aspose.Zip](/zip/python-net/)

