---
title: "WimArchive"
second_title: "Aspose.Zip для Python через .NET Справочник API"
description: 
type: docs
weight: 10
url: /ru/python-net/aspose.zip.wim/wimarchive/
---

## WimArchive class

Этот класс представляет файл архива wim.

Тип WimArchive раскрывает следующие члены:
## Конструкторы
| Имя | Описание |
| :- | :- |
| WimArchive(source_stream, load_options) | Инициализирует новый экземпляр класса [WimArchive](/zip/python-net/aspose.zip.wim/wimarchive/) и формирует список записей, которые можно извлечь из архива. |
| WimArchive(path, load_options) | Инициализирует новый экземпляр класса [WimArchive](/zip/python-net/aspose.zip.wim/wimarchive/) и формирует список записей, которые можно извлечь из архива. |
## Свойства
| Имя | Описание |
| :- | :- |
| images | Получает записи типа [WimImage](/zip/python-net/aspose.zip.wim/wimimage/), составляющие архив. |
| entries | Получает записи типа [WimEntry](/zip/python-net/aspose.zip.wim/wimentry/), составляющие архив. |
| guid | Получает идентифицирующий GUID архива. |
| boot_image_index | Получает (нумерацию с нуля) индекс загрузочного образа. |
| file_format_version | Получает версию формата файла. |
| manifest | Получает встроенный манифест, описывающий файл и содержащиеся в нём образы. |
| file_entries | Получает записи типа [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/), составляющие архив. |
| format | Возвращает формат архива. |
## Методы
| Имя | Описание |
| :- | :- |
| extract_to_directory(destination_directory) | Извлекает архив в файл по пути. |

### См. также

* namespace [aspose.zip.wim](/zip/python-net/aspose.zip.wim/)
* assembly [Aspose.Zip](/zip/python-net/)

