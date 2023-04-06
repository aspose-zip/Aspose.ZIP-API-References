---
title: Class GzipArchive
second_title: Aspose.ZIP для справочника API .NET
description: Aspose.Zip.Gzip.GzipArchive сорт. Этот класс представляет архивный файл gzip. Используйте его для создания или извлечения архивов gzip.
type: docs
weight: 210
url: /ru/net/aspose.zip.gzip/gziparchive/
---
## GzipArchive class

Этот класс представляет архивный файл gzip. Используйте его для создания или извлечения архивов gzip.

```csharp
public class GzipArchive : IArchive, IArchiveFileEntry
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GzipArchive](gziparchive/#constructor)() | Инициализирует новый экземпляр`GzipArchive` класс подготовлен к сжатию. |
| [GzipArchive](gziparchive/#constructor_1)(Stream, bool) | Инициализирует новый экземпляр`GzipArchive` класс подготовлен к распаковке. |
| [GzipArchive](gziparchive/#constructor_2)(string, bool) | Инициализирует новый экземпляр`GzipArchive` класс. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [Name](../../aspose.zip.gzip/gziparchive/name/) { get; } | Имя исходного файла. |

## Методы

| Имя | Описание |
| --- | --- |
| [Dispose](../../aspose.zip.gzip/gziparchive/dispose/)() | Выполняет определяемые приложением задачи, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/)(Stream) | Извлекает архив в указанный поток. |
| [Open](../../aspose.zip.gzip/gziparchive/open/)() | Открывает архив для извлечения и предоставляет поток с содержимым архива. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save)(Stream) | Сохраняет архив в указанный поток. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save_1)(string) | Сохраняет архив в указанный файл назначения. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_1)(FileInfo) | Задает сжатие содержимого внутри архива. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_2)(Stream) | Задает сжатие содержимого внутри архива. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_3)(string) | Задает сжатие содержимого внутри архива. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource)(TarArchive) | Задает сжатие содержимого внутри архива. |

### Примечания

Алгоритм сжатия Gzip основан на алгоритме DEFLATE, который представляет собой комбинацию LZ77 и кодирования Хаффмана.

### Смотрите также

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* пространство имен [Aspose.Zip.Gzip](../../aspose.zip.gzip/)
* сборка [Aspose.Zip](../../)


