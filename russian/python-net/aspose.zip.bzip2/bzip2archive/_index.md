---
title: "Bzip2Archive"
second_title: "Aspose.Zip для Python через .NET Справочник API"
description: 
type: docs
weight: 10
url: /ru/python-net/aspose.zip.bzip2/bzip2archive/
---

## Bzip2Archive class

Этот класс представляет файл архива bzip2. Используйте его для создания или извлечения архивов bzip2.

Тип Bzip2Archive раскрывает следующие члены:
## Конструкторы
| Имя | Описание |
| :- | :- |
| Bzip2Archive() | Создаёт новый экземпляр класса [Bzip2Archive](/zip/python-net/aspose.zip.bzip2/bzip2archive/) для сжатия. |
| Bzip2Archive(source_stream, load_options) | Создаёт новый экземпляр класса [Bzip2Archive](/zip/python-net/aspose.zip.bzip2/bzip2archive/) для распаковки. |
| Bzip2Archive(path, load_options) | Создаёт новый экземпляр класса [Bzip2Archive](/zip/python-net/aspose.zip.bzip2/bzip2archive/) для распаковки. |
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
| set_source(source) | Устанавливает содержимое, которое будет сжато в архиве. |
| set_source(file_info) | Устанавливает содержимое, которое будет сжато в архиве. |
| set_source(path) | Устанавливает содержимое, которое будет сжато в архиве. |
| set_source(tar_archive, format) | Устанавливает содержимое, которое будет сжато в архиве. |
| set_source(cpio_archive, format) | Устанавливает содержимое, которое будет сжато в архиве. |
| extract(destination) | Извлекает архив в предоставленный поток. |
| extract(path) | Извлекает содержимое архива в предоставленный каталог. |
| save(output_stream, save_options) | Сохраняет архив в предоставленный поток. |
| save(destination_file_name, save_options) | Сохраняет архив в указанный файл назначения. |
| open() | Открывает архив для извлечения и предоставляет поток с содержимым архива. |
| extract_to_directory(destination_directory) | Извлекает содержимое архива в предоставленный каталог. |

### См. также

* namespace [aspose.zip.bzip2](/zip/python-net/aspose.zip.bzip2/)
* assembly [Aspose.Zip](/zip/python-net/)

