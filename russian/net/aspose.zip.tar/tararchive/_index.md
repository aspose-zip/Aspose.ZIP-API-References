---
title: "Класс TarArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Tar.TarArchive. Этот класс представляет файл tar-архива. Используйте его для создания, извлечения или обновления tar-архивов"
type: docs
weight: 1270
url: /ru/net/aspose.zip.tar/tararchive/
---
## TarArchive class

Этот класс представляет файл архива tar. Используйте его для создания, извлечения или обновления архивов tar.

```csharp
public class TarArchive : IArchive
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TarArchive](tararchive/#constructor)() | Инициализирует новый экземпляр класса `TarArchive`. |
| [TarArchive](tararchive/#constructor_1)(Stream, TarLoadOptions) | Инициализирует новый экземпляр класса `TarArchive` и формирует список записей, которые могут быть извлечены из архива. |
| [TarArchive](tararchive/#constructor_2)(string, TarLoadOptions) | Инициализирует новый экземпляр класса `TarArchive` и формирует список записей, которые могут быть извлечены из архива. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Entries](../../aspose.zip.tar/tararchive/entries/) { get; } | Получает записи типа [`TarEntry`](../tarentry/), составляющие архив. |

## Методы

| Имя | Описание |
| --- | --- |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip)(Stream) | Извлекает предоставленный gzip-архив и формирует `TarArchive` из извлечённых данных. |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip_1)(string) | Извлекает предоставленный gzip-архив и формирует `TarArchive` из извлечённых данных. |
| static [FromLZ4](../../aspose.zip.tar/tararchive/fromlz4/#fromlz4)(Stream) | Извлекает предоставленный LZ4-архив и формирует `TarArchive` из извлечённых данных. |
| static [FromLZ4](../../aspose.zip.tar/tararchive/fromlz4/#fromlz4_1)(string) | Извлекает предоставленный LZ4-архив и формирует `TarArchive` из извлечённых данных. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip)(Stream) | Извлекает предоставленный lzip-архив и формирует `TarArchive` из извлечённых данных. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip_1)(string) | Извлекает предоставленный lzip-архив и формирует `TarArchive` из извлечённых данных. |
| static [FromLZMA](../../aspose.zip.tar/tararchive/fromlzma/#fromlzma)(Stream) | Извлекает предоставленный LZMA-архив и формирует `TarArchive` из извлечённых данных. |
| static [FromLZMA](../../aspose.zip.tar/tararchive/fromlzma/#fromlzma_1)(string) | Извлекает предоставленный LZMA-архив и формирует `TarArchive` из извлечённых данных. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz)(Stream) | Извлекает предоставленный архив формата xz и формирует `TarArchive` из извлечённых данных. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz_1)(string) | Извлекает предоставленный архив формата xz и формирует `TarArchive` из извлечённых данных. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz)(Stream) | Извлекает предоставленный архив формата Z и формирует `TarArchive` из извлечённых данных. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz_1)(string) | Извлекает предоставленный архив формата Z и формирует `TarArchive` из извлечённых данных. |
| static [FromZstandard](../../aspose.zip.tar/tararchive/fromzstandard/#fromzstandard)(Stream) | Извлекает предоставленный Zstandard-архив и формирует `TarArchive` из извлечённых данных. |
| static [FromZstandard](../../aspose.zip.tar/tararchive/fromzstandard/#fromzstandard_1)(string) | Извлекает предоставленный Zstandard-архив и формирует `TarArchive` из извлечённых данных. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries)(DirectoryInfo, bool) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries_1)(string, bool) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry)(string, FileInfo, bool) | Создаёт одну запись внутри архива. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_1)(string, Stream, FileSystemInfo) | Создаёт одну запись внутри архива. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_2)(string, string, bool) | Создаёт одну запись внутри архива. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry_1)(int) | Удаляет запись из списка записей по индексу. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry)(TarEntry) | Удаляет первое вхождение конкретной записи из списка записей. |
| [Dispose](../../aspose.zip.tar/tararchive/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [ExtractToDirectory](../../aspose.zip.tar/tararchive/extracttodirectory/)(string) | Извлекает все файлы из архива в указанный каталог. |
| [Save](../../aspose.zip.tar/tararchive/save/#save)(Stream, TarFormat?) | Сохраняет архив в предоставленный поток. |
| [Save](../../aspose.zip.tar/tararchive/save/#save_1)(string, TarFormat?) | Сохраняет архив в указанный файл назначения. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped)(Stream, TarFormat?) | Сохраняет архив в поток с gzip‑сжатием. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped_1)(string, TarFormat?) | Сохраняет архив в файл по пути с gzip‑сжатием. |
| [SaveLZ4Compressed](../../aspose.zip.tar/tararchive/savelz4compressed/#savelz4compressed)(Stream, TarFormat?) | Сохраняет архив в поток с LZ4‑сжатием. |
| [SaveLZ4Compressed](../../aspose.zip.tar/tararchive/savelz4compressed/#savelz4compressed_1)(string, TarFormat?) | Сохраняет архив в файл по пути с LZ4‑сжатием. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped)(Stream, TarFormat?) | Сохраняет архив в поток с lzip‑сжатием. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped_1)(string, TarFormat?) | Сохраняет архив в файл по пути с lzip‑сжатием. |
| [SaveLZMACompressed](../../aspose.zip.tar/tararchive/savelzmacompressed/#savelzmacompressed)(Stream, TarFormat?) | Сохраняет архив в поток с LZMA‑сжатием. |
| [SaveLZMACompressed](../../aspose.zip.tar/tararchive/savelzmacompressed/#savelzmacompressed_1)(string, TarFormat?) | Сохраняет архив в файл по пути с lzma‑сжатием. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed)(Stream, TarFormat?, XzArchiveSettings) | Сохраняет архив в поток с xz‑сжатием. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed_1)(string, TarFormat?, XzArchiveSettings) | Сохраняет архив по указанному пути с xz‑сжатием. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed)(Stream, TarFormat?) | Сохраняет архив в поток с Z‑сжатием. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed_1)(string, TarFormat?) | Сохраняет архив по указанному пути с Z‑сжатием |
| [SaveZstandard](../../aspose.zip.tar/tararchive/savezstandard/#savezstandard)(Stream, TarFormat?) | Сохраняет архив в поток с компрессией Zstandard. |
| [SaveZstandard](../../aspose.zip.tar/tararchive/savezstandard/#savezstandard_1)(string, TarFormat?) | Сохраняет архив в файл по пути с компрессией Zstandard. |

### См. также

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Tar](../../aspose.zip.tar/)
* assembly [Aspose.Zip](../../)


