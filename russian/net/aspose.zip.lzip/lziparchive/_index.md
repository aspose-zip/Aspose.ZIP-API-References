---
title: "Класс LzipArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Lzip.LzipArchive. Этот класс представляет файл Lzip-архива. Используйте его для создания или извлечения Lzip-архивов"
type: docs
weight: 700
url: /ru/net/aspose.zip.lzip/lziparchive/
---
## LzipArchive class

Этот класс представляет файл архива Lzip. Используйте его для создания или извлечения архивов Lzip.

```csharp
public class LzipArchive : IArchive, IArchiveFileEntry
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [LzipArchive](lziparchive/#constructor)(LzipArchiveSettings) | Инициализирует новый экземпляр `LzipArchive`. |
| [LzipArchive](lziparchive/#constructor_1)(Stream, LzipLoadOptions) | Инициализирует новый экземпляр класса `LzipArchive`, подготовленный для распаковки. |
| [LzipArchive](lziparchive/#constructor_2)(string, LzipLoadOptions) | Инициализирует новый экземпляр класса `LzipArchive`, подготовленный для распаковки. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Settings](../../aspose.zip.lzip/lziparchive/settings/) { get; } | Получает настройки конкретного lzip-архива. |
| [UncompressedSize](../../aspose.zip.lzip/lziparchive/uncompressedsize/) { get; } | Несжатый размер данных файла в байтах. |

## Методы

| Имя | Описание |
| --- | --- |
| [Dispose](../../aspose.zip.lzip/lziparchive/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [Extract](../../aspose.zip.lzip/lziparchive/extract/#extract)(FileInfo) | Извлекает lzip-архив в файл. |
| [Extract](../../aspose.zip.lzip/lziparchive/extract/#extract_1)(Stream) | Извлекает lzip-архив в поток. |
| [Extract](../../aspose.zip.lzip/lziparchive/extract/#extract_2)(string) | Извлекает lzip-архив в файл по пути. |
| [ExtractToDirectory](../../aspose.zip.lzip/lziparchive/extracttodirectory/)(string) | Извлекает содержимое архива в указанную директорию. |
| [Save](../../aspose.zip.lzip/lziparchive/save/#save)(FileInfo) | Сохраняет lzip-архив в указанный файл назначения. |
| [Save](../../aspose.zip.lzip/lziparchive/save/#save_1)(Stream) | Сохраняет lzip-архив в указанный поток. |
| [Save](../../aspose.zip.lzip/lziparchive/save/#save_2)(string) | Сохраняет lzip-архив в указанный файл назначения. |
| [SetSource](../../aspose.zip.lzip/lziparchive/setsource/#setsource)(FileInfo) | Устанавливает содержимое, которое будет сжато в архиве. |
| [SetSource](../../aspose.zip.lzip/lziparchive/setsource/#setsource_1)(Stream) | Устанавливает содержимое, которое будет сжато в архиве. |
| [SetSource](../../aspose.zip.lzip/lziparchive/setsource/#setsource_2)(string) | Устанавливает содержимое, которое будет сжато в архиве. |

### См. также

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Lzip](../../aspose.zip.lzip/)
* assembly [Aspose.Zip](../../)


