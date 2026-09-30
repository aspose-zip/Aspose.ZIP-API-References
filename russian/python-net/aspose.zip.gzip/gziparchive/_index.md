---
title: "GzipArchive"
second_title: "Aspose.Zip для Python через .NET Справочник API"
description: 
type: docs
weight: 10
url: /ru/python-net/aspose.zip.gzip/gziparchive/
---

## GzipArchive class

Этот класс представляет файл архива gzip. Используйте его для создания или извлечения архивов gzip.

Тип GzipArchive раскрывает следующие члены:
## Конструкторы
| Имя | Описание |
| :- | :- |
| GzipArchive() | Инициализирует новый экземпляр класса [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/), подготовленного для сжатия. |
| GzipArchive(source_stream, parse_header) | Инициализирует новый экземпляр класса [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/), подготовленного для распаковки. |
| GzipArchive(source_stream, options) | Инициализирует новый экземпляр класса [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/), подготовленного для распаковки. |
| GzipArchive(path, options) | Инициализирует новый экземпляр класса [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/), подготовленного для распаковки. |
| GzipArchive(path, parse_header) | Инициализирует новый экземпляр класса [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/), подготовленного для распаковки. |
## Свойства
| Имя | Описание |
| :- | :- |
| uncompressed_size | Получает размер оригинального файла. |
| name | Имя оригинального файла. |
| file_entries | Получает записи типа [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/), составляющие архив. |
| format | Возвращает формат архива. |
| length | Получает длину записи в байтах. |
## Методы
| Имя | Описание |
| :- | :- |
| set_source(source) | Устанавливает содержимое, которое будет сжато в архиве. |
| set_source(file_info) | Устанавливает содержимое, которое будет сжато в архиве. |
| set_source(path) | Устанавливает содержимое, которое будет сжато в архиве. |
| set_source(tar_archive) | Устанавливает содержимое, которое будет сжато в архиве. |
| extract(destination) | Извлекает архив в предоставленный поток. |
| extract(path) | Извлекает содержимое архива в предоставленный каталог. |
| save(output_stream) | Сохраняет архив в предоставленный поток. |
| save(destination_file_name) | Сохраняет архив в указанный файл назначения. |
| open() | Открывает архив для извлечения и предоставляет поток с содержимым архива. |
| extract_to_directory(destination_directory) | Извлекает содержимое архива в предоставленный каталог. |

### См. также

* namespace [aspose.zip.gzip](/zip/python-net/aspose.zip.gzip/)
* assembly [Aspose.Zip](/zip/python-net/)

