---
title: "Lz4Archive"
second_title: "Aspose.Zip для Python через .NET Справочник API"
description: 
type: docs
weight: 10
url: /ru/python-net/aspose.zip.lz4/lz4archive/
---

## Lz4Archive class

Этот класс представляет файл архива LZ4. Используйте его для извлечения или создания архивов LZ4.

Тип Lz4Archive раскрывает следующие члены:
## Конструкторы
| Имя | Описание |
| :- | :- |
| Lz4Archive(source_stream, load_options) | Инициализирует новый экземпляр класса [Lz4Archive](/zip/python-net/aspose.zip.lz4/lz4archive/) для распаковки. |
| Lz4Archive(path, load_options) | Инициализирует новый экземпляр класса [Lz4Archive](/zip/python-net/aspose.zip.lz4/lz4archive/). |
| Lz4Archive(settings) | Инициализирует новый экземпляр класса [Lz4Archive](/zip/python-net/aspose.zip.lz4/lz4archive/) подготовленного для сжатия. |
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
| extract(path) | Извлекает архив в файл по пути. |
| extract(destination) | Извлекает архив в предоставленный поток. |
| save(output) | Сохраняет lz4 архив в предоставленный поток. |
| save(destination) | Сохраняет lz4 архив в предоставленный файл назначения. |
| save(destination_file_name) | Сохраняет архив в указанный файл назначения. |
| set_source(source) | Устанавливает содержимое, которое будет сжато в архиве. |
| set_source(file_info) | Устанавливает содержимое, которое будет сжато в архиве. |
| set_source(tar_archive, format) | Устанавливает содержимое, которое будет сжато в архиве. |
| set_source(path) | Устанавливает содержимое, которое будет сжато в архиве. |
| extract_to_directory(destination_directory) | Извлекает содержимое архива в предоставленный каталог. |
| open() | Открывает архив для извлечения и предоставляет поток с содержимым архива. |

### См. также

* namespace [aspose.zip.lz4](/zip/python-net/aspose.zip.lz4/)
* assembly [Aspose.Zip](/zip/python-net/)

