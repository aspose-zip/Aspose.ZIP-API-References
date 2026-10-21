---
title: "LzipArchive"
second_title: "Aspose.Zip для Python через .NET Справочник API"
description: 
type: docs
weight: 10
url: /ru/python-net/aspose.zip.lzip/lziparchive/
---

## LzipArchive class

Этот класс представляет файл архива Lzip. Используйте его для создания или извлечения архивов Lzip.

Тип LzipArchive раскрывает следующие члены:
## Конструкторы
| Имя | Описание |
| :- | :- |
| LzipArchive(settings) | Инициализирует новый экземпляр [LzipArchive](/zip/python-net/aspose.zip.lzip/lziparchive/). |
| LzipArchive(source_stream, options) | Инициализирует новый экземпляр класса [LzipArchive](/zip/python-net/aspose.zip.lzip/lziparchive/), подготовленный для распаковки. |
| LzipArchive(path, options) | Инициализирует новый экземпляр класса [LzipArchive](/zip/python-net/aspose.zip.lzip/lziparchive/), подготовленный для распаковки. |
## Свойства
| Имя | Описание |
| :- | :- |
| uncompressed_size | Несжатый размер данных файла в байтах. |
| settings | Получает настройки конкретного lzip-архива. |
| file_entries | Получает записи типа [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/), составляющие архив. |
| format | Возвращает формат архива. |
| name | Получает имя записи. |
| length | Получает длину записи в байтах. |
## Методы
| Имя | Описание |
| :- | :- |
| extract(destination) | Извлекает lzip-архив в поток. |
| extract(file_info) | Извлекает lzip-архив в файл. |
| extract(path) | Извлекает lzip‑архив в файл по пути. |
| save(output_stream) | Сохраняет lzip‑архив в указанный поток. |
| save(destination_file_name) | Сохраняет lzip‑архив в указанный файл назначения. |
| save(destination) | Сохраняет lzip‑архив в указанный файл назначения. |
| set_source(source) | Устанавливает содержимое, которое будет сжато в архиве. |
| set_source(file_info) | Устанавливает содержимое, которое будет сжато в архиве. |
| set_source(path) | Устанавливает содержимое, которое будет сжато в архиве. |
| extract_to_directory(destination_directory) | Извлекает содержимое архива в предоставленный каталог. |

### См. также

* namespace [aspose.zip.lzip](/zip/python-net/aspose.zip.lzip/)
* assembly [Aspose.Zip](/zip/python-net/)

