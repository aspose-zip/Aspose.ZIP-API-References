---
title: "Класс GzipArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Gzip.GzipArchive. Этот класс представляет файл gzip-архива. Используйте его для создания или извлечения gzip-архивов"
type: docs
weight: 510
url: /ru/net/aspose.zip.gzip/gziparchive/
---
## GzipArchive class

Этот класс представляет файл архива gzip. Используйте его для создания или извлечения архивов gzip.

```csharp
public class GzipArchive : IArchive, IArchiveFileEntry
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GzipArchive](gziparchive/#constructor)() | Инициализирует новый экземпляр класса `GzipArchive`, подготовленный для сжатия. |
| [GzipArchive](gziparchive/#constructor_2)(Stream, bool) | Инициализирует новый экземпляр класса `GzipArchive`, подготовленный для распаковки. |
| [GzipArchive](gziparchive/#constructor_1)(Stream, GzipLoadOptions) | Инициализирует новый экземпляр класса `GzipArchive`, подготовленный для распаковки. |
| [GzipArchive](gziparchive/#constructor_4)(string, bool) | Инициализирует новый экземпляр класса `GzipArchive`, подготовленный для распаковки. |
| [GzipArchive](gziparchive/#constructor_3)(string, GzipLoadOptions) | Инициализирует новый экземпляр класса `GzipArchive`, подготовленный для распаковки. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Name](../../aspose.zip.gzip/gziparchive/name/) { get; } | Имя оригинального файла. |
| [UncompressedSize](../../aspose.zip.gzip/gziparchive/uncompressedsize/) { get; } | Получает размер оригинального файла. |

## Методы

| Имя | Описание |
| --- | --- |
| [Dispose](../../aspose.zip.gzip/gziparchive/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/#extract_1)(Stream) | Извлекает архив в предоставленный поток. |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/#extract)(string) | Извлекает архив в файл по указанному пути. |
| [ExtractToDirectory](../../aspose.zip.gzip/gziparchive/extracttodirectory/)(string) | Извлекает содержимое архива в указанную директорию. |
| [Open](../../aspose.zip.gzip/gziparchive/open/)() | Открывает архив для извлечения и предоставляет поток с содержимым архива. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save)(Stream) | Сохраняет архив в предоставленный поток. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save_1)(string) | Сохраняет архив в указанный файл назначения. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_1)(FileInfo) | Устанавливает содержимое, которое будет сжато в архиве. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_2)(Stream) | Устанавливает содержимое, которое будет сжато в архиве. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_3)(string) | Устанавливает содержимое, которое будет сжато в архиве. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource)(TarArchive) | Устанавливает содержимое, которое будет сжато в архиве. |

## Примечания

Алгоритм сжатия Gzip основан на алгоритме DEFLATE, который представляет собой комбинацию LZ77 и кодирования Хаффмана.

### См. также

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Gzip](../../aspose.zip.gzip/)
* assembly [Aspose.Zip](../../)


