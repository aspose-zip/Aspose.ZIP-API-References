---
title: "Класс WimDirectoryEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Wim.WimDirectoryEntry. Представляет один каталог внутри архива wim."
type: docs
weight: 1340
url: /ru/net/aspose.zip.wim/wimdirectoryentry/
---
## WimDirectoryEntry class

Представляет отдельный каталог внутри архива wim.

```csharp
public sealed class WimDirectoryEntry : WimEntry
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AllEntries](../../aspose.zip.wim/wimdirectoryentry/allentries/) { get; } | Получает все записи типа [`WimEntry`](../wimentry/), рекурсивно составляющие каталог. |
| [AlternateDataStreams](../../aspose.zip.wim/wimentry/alternatedatastreams/) { get; } | Получает имена альтернативных потоков данных для файла или каталога. |
| [Archive](../../aspose.zip.wim/wimentry/archive/) { get; } | Получает архив, к которому принадлежит запись. |
| [ChangeTime](../../aspose.zip.wim/wimentry/changetime/) { get; } | Получает время последнего изменения файла или каталога. |
| [CreationTime](../../aspose.zip.wim/wimentry/creationtime/) { get; } | Получает время создания файла или каталога. |
| [Directories](../../aspose.zip.wim/wimdirectoryentry/directories/) { get; } | Получает записи типа `WimDirectoryEntry`, составляющие каталог. |
| [FileAttributes](../../aspose.zip.wim/wimentry/fileattributes/) { get; } | Получает атрибуты файла или каталога. |
| [Files](../../aspose.zip.wim/wimdirectoryentry/files/) { get; } | Получает записи типа [`WimFileEntry`](../wimfileentry/), составляющие каталог. |
| [FilesAndDirectories](../../aspose.zip.wim/wimdirectoryentry/filesanddirectories/) { get; } | Получает элементы типа [`WimEntry`](../wimentry/), составляющие каталог. |
| [FullPath](../../aspose.zip.wim/wimentry/fullpath/) { get; } | Получает полный путь записи внутри образа. |
| [HardLink](../../aspose.zip.wim/wimentry/hardlink/) { get; } | Получает идентификатор жесткой ссылки файла или каталога. |
| [HasHardLinks](../../aspose.zip.wim/wimentry/hashardlinks/) { get; } | Получает, известен ли файл или каталог под другими именами. |
| [Image](../../aspose.zip.wim/wimentry/image/) { get; } | Получает образ, к которому принадлежит запись. |
| [IsDirectory](../../aspose.zip.wim/wimentry/isdirectory/) { get; } | Возвращает значение, указывающее, является ли запись каталогом. |
| [LastAccessTime](../../aspose.zip.wim/wimentry/lastaccesstime/) { get; } | Получает время последнего доступа к файлу или каталогу. |
| [ModificationTime](../../aspose.zip.wim/wimentry/modificationtime/) { get; } | Получает время изменения файла или каталога. |
| [Name](../../aspose.zip.wim/wimentry/name/) { get; } | Получает имя записи внутри образа. |
| [Parent](../../aspose.zip.wim/wimentry/parent/) { get; } | Получает родительский каталог, к которому относится запись. |
| [ShortName](../../aspose.zip.wim/wimentry/shortname/) { get; } | Получает короткое имя записи внутри образа. |

## Методы

| Имя | Описание |
| --- | --- |
| [ExtractToDirectory](../../aspose.zip.wim/wimdirectoryentry/extracttodirectory/)(string) | Извлекает все файлы из текущего каталога в указанный каталог. |
| override [ToString](../../aspose.zip.wim/wimentry/tostring/)() |  |

### См. также

* class [WimEntry](../wimentry/)
* namespace [Aspose.Zip.Wim](../../aspose.zip.wim/)
* assembly [Aspose.Zip](../../)


