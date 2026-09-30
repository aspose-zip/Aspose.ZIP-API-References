---
title: "SevenZipLZMACompressionSettings"
second_title: "Aspose.Zip для Python через .NET Справочник API"
description: 
type: docs
weight: 210
url: /ru/python-net/aspose.zip.saving/sevenziplzmacompressionsettings/
---

## SevenZipLZMACompressionSettings class

Настройки метода сжатия LZMA внутри 7z-архива.

Тип SevenZipLZMACompressionSettings раскрывает следующие члены:
## Конструкторы
| Имя | Описание |
| :- | :- |
| SevenZipLZMACompressionSettings() | Инициализирует новый экземпляр класса [SevenZipLZMACompressionSettings](/zip/python-net/aspose.zip.saving/sevenziplzmacompressionsettings/) с параметрами по умолчанию. |
| SevenZipLZMACompressionSettings(dictionary_size, number_of_fast_bytes, literal_context_bits) | Инициализирует новый экземпляр класса SevenZipLZMACompressionSettings |
| SevenZipLZMACompressionSettings(dictionary_size) | Инициализирует новый экземпляр класса SevenZipLZMACompressionSettings |
## Свойства
| Имя | Описание |
| :- | :- |
| метод | Получает метод сжатия или распаковки. |
| dictionary_size | Размер словаря (буфера истории) указывает, сколько байтов недавно обработанных несжатых данных хранится в памяти.<br/>            Если не задан, будет выбран в зависимости от размера записи. Должен быть от 4096 до 1073741824, либо равен нулю для автоматического определения на основе размера записи. |
| number_of_fast_bytes | Получает количество байтов, используемых для быстрого поиска совпадений в алгоритме LZMA. |
| literal_context_bits | Получает количество битов контекста литералов. |

### См. также

* namespace [aspose.zip.saving](/zip/python-net/aspose.zip.saving/)
* assembly [Aspose.Zip](/zip/python-net/)

