---
title: "UueArchive"
second_title: "Aspose.Zip для Python через .NET Справочник API"
description: 
type: docs
weight: 10
url: /ru/python-net/aspose.zip.uue/uuearchive/
---

## UueArchive class

Этот класс представляет uuencoded файл.

Тип UueArchive предоставляет следующие члены:
## Конструкторы
| Имя | Описание |
| :- | :- |
| UueArchive() | Инициализирует новый экземпляр класса [UueArchive](/zip/python-net/aspose.zip.uue/uuearchive/) подготовленного для кодирования. |
| UueArchive(source_stream) | Инициализирует новый экземпляр класса [UueArchive](/zip/python-net/aspose.zip.uue/uuearchive/), подготовленного для декодирования. |
| UueArchive(path) | Инициализирует новый экземпляр класса [UueArchive](/zip/python-net/aspose.zip.uue/uuearchive/). |
## Свойства
| Имя | Описание |
| :- | :- |
| name | Имя оригинального файла. |
| file_entries | Получает записи типа [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/), составляющие архив. |
| format | Возвращает формат архива. |
| length | Получает длину записи в байтах. |
## Методы
| Имя | Описание |
| :- | :- |
| save(output_stream, save_options) | Сохраняет архив в предоставленный поток. |
| save(destination_file_name, save_options) | Сохраняет архив в указанный файл назначения. |
| extract(destination) | Извлекает архив в предоставленный поток. |
| extract(path) | Извлекает архив в файл по пути. |
| set_source(source) | Устанавливает содержимое, которое будет закодировано в архиве. |
| set_source(file_info) | Устанавливает содержимое, которое будет сжато в архиве. |
| set_source(path) | Устанавливает содержимое, которое будет закодировано в архиве. |
| extract_to_directory(destination_directory) | Извлекает содержимое архива в предоставленный каталог. |
| open() | Открывает архив для декодирования и предоставляет поток с содержимым архива. |

### См. также

* namespace [aspose.zip.uue](/zip/python-net/aspose.zip.uue/)
* assembly [Aspose.Zip](/zip/python-net/)

