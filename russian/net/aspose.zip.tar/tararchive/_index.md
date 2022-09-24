---
title: TarArchive
second_title: Aspose.ZIP для справочника API .NET
description: Этот класс представляет файл архива tar. Используйте его для создания извлечения или обновления tarархивов.
type: docs
weight: 600
url: /ru/net/aspose.zip.tar/tararchive/
---
## TarArchive class

Этот класс представляет файл архива tar. Используйте его для создания, извлечения или обновления tar-архивов.

```csharp
public class TarArchive : IDisposable
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TarArchive](tararchive#constructor)() | Инициализирует новый экземпляр[`TarArchive`](../tararchive) класс. |
| [TarArchive](tararchive#constructor_1)(Stream) | Инициализирует новый экземпляр[`Archive`](../../aspose.zip/archive) список записей классов и композиций можно извлечь из архива. |
| [TarArchive](tararchive#constructor_2)(string) | Инициализирует новый экземпляр[`TarArchive`](../tararchive) список записей классов и композиций можно извлечь из архива. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [Entries](../../aspose.zip.tar/tararchive/entries) { get; } | Получает записи[`TarEntry`](../tarentry) тип составляющий архив. |

## Методы

| Имя | Описание |
| --- | --- |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip#fromgzip)(Stream) | Распаковывает прилагаемый архив gzip и компонует[`TarArchive`](../tararchive) из извлеченных данных. |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip#fromgzip_1)(string) | Распаковывает прилагаемый архив gzip и компонует[`TarArchive`](../tararchive) из извлеченных данных. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip#fromlzip)(Stream) | Распаковывает прилагаемый lzip-архив и компонует[`TarArchive`](../tararchive) из извлеченных данных. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip#fromlzip_1)(string) | Распаковывает прилагаемый lzip-архив и компонует[`TarArchive`](../tararchive) из извлеченных данных. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz#fromxz)(Stream) | Распаковывает прилагаемый архив формата xz и компонует[`TarArchive`](../tararchive) из извлеченных данных. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz#fromxz_1)(string) | Распаковывает прилагаемый архив формата xz и компонует[`TarArchive`](../tararchive) из извлеченных данных. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz#fromz)(Stream) | Распаковывает прилагаемый архив формата Z и компонует[`TarArchive`](../tararchive) из извлеченных данных. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz#fromz_1)(string) | Распаковывает прилагаемый архив формата Z и компонует[`TarArchive`](../tararchive) из извлеченных данных. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries#createentries)(DirectoryInfo, bool) | Добавляет в архив все файлы и каталоги рекурсивно в заданном каталоге. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries#createentries_1)(string, bool) | Добавляет в архив все файлы и каталоги рекурсивно в заданном каталоге. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry#createentry)(string, FileInfo, bool) | Создать одну запись в архиве. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry#createentry_1)(string, Stream, FileSystemInfo) | Создать одну запись в архиве. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry#createentry_2)(string, string, bool) | Создать одну запись в архиве. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry#deleteentry_1)(int) | Удаляет запись из списка записей по индексу. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry#deleteentry)(TarEntry) | Удаляет первое вхождение определенной записи из списка записей. |
| [Dispose](../../aspose.zip.tar/tararchive/dispose)() | Выполняет определяемые приложением задачи, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [ExtractToDirectory](../../aspose.zip.tar/tararchive/extracttodirectory)(string) | Извлекает все файлы из архива в указанный каталог. |
| [Save](../../aspose.zip.tar/tararchive/save#save)(Stream, TarFormat?) | Сохраняет архив в указанный поток. |
| [Save](../../aspose.zip.tar/tararchive/save#save_1)(string, TarFormat?) | Сохраняет архив в указанный файл назначения. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped#savegzipped)(Stream, TarFormat?) | Сохраняет архив в поток со сжатием gzip. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped#savegzipped_1)(string, TarFormat?) | Сохраняет архив в файл по пути со сжатием gzip. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped#savelzipped)(Stream, TarFormat?) | Сохраняет архив в поток со сжатием lzip. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped#savelzipped_1)(string, TarFormat?) | Сохраняет архив в файл по пути со сжатием lzip. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed#savexzcompressed)(Stream, TarFormat?, XzArchiveSettings) | Сохраняет архив в поток со сжатием xz. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed#savexzcompressed_1)(string, TarFormat?, XzArchiveSettings) | Сохраняет архив в путь по пути со сжатием xz. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed#savezcompressed)(Stream, TarFormat?) | Сохраняет архив в поток с Z-сжатием. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed#savezcompressed_1)(string, TarFormat?) | Сохраняет архив в путь по пути с Z-сжатием. |

### Смотрите также

* пространство имен [Aspose.Zip.Tar](../../aspose.zip.tar)
* сборка [Aspose.Zip](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
