---
title: "Класс TarEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Tar.TarEntry. Представляет отдельный файл внутри tar-архива"
type: docs
weight: 1280
url: /ru/net/aspose.zip.tar/tarentry/
---
## TarEntry class

Представляет отдельный файл в архиве tar.

```csharp
public class TarEntry : IArchiveFileEntry
```

## Свойства

| Имя | Описание |
| --- | --- |
| [IsDirectory](../../aspose.zip.tar/tarentry/isdirectory/) { get; } | Возвращает значение, указывающее, является ли запись каталогом. |
| [Length](../../aspose.zip.tar/tarentry/length/) { get; } | Получить длину записи в байтах. |
| [ModificationTime](../../aspose.zip.tar/tarentry/modificationtime/) { get; } | Получает время изменения файла или каталога. |
| [Name](../../aspose.zip.tar/tarentry/name/) { get; set; } | Получает или задает имя записи в архиве. |
| [UncompressedSize](../../aspose.zip.tar/tarentry/uncompressedsize/) { get; } | Получает размер оригинального файла. |

## Методы

| Имя | Описание |
| --- | --- |
| [Extract](../../aspose.zip.tar/tarentry/extract/#extract_1)(Stream) | Извлекает запись в предоставленный поток. |
| [Extract](../../aspose.zip.tar/tarentry/extract/#extract)(string) | Извлекает запись в файловую систему по указанному пути. |
| [Open](../../aspose.zip.tar/tarentry/open/)() | Открывает запись для извлечения и предоставляет поток с содержимым записи. |

### См. также

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Tar](../../aspose.zip.tar/)
* assembly [Aspose.Zip](../../)


