---
title: "Класс XarDirectoryEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Aspose.Zip.Xar.XarDirectoryEntry класс. Представляет запись каталога в архиве xar"
type: docs
weight: 1450
url: /ru/net/aspose.zip.xar/xardirectoryentry/
---
## XarDirectoryEntry class

Представляет запись каталога внутри архива xar.

```csharp
public sealed class XarDirectoryEntry : XarEntry
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AllEntries](../../aspose.zip.xar/xardirectoryentry/allentries/) { get; } | Получает все записи типа [`XarEntry`](../xarentry/), составляющие каталог рекурсивно. |
| [CreationTime](../../aspose.zip.xar/xarentry/creationtime/) { get; } | Получает время создания файла или каталога. |
| [Directories](../../aspose.zip.xar/xardirectoryentry/directories/) { get; } | Получает записи типа `XarDirectoryEntry`, составляющие каталог. |
| [Files](../../aspose.zip.xar/xardirectoryentry/files/) { get; } | Получает записи типа [`XarFileEntry`](../xarfileentry/), составляющие каталог. |
| [FilesAndDirectories](../../aspose.zip.xar/xardirectoryentry/filesanddirectories/) { get; } | Получает записи типа [`XarEntry`](../xarentry/), составляющие каталог. |
| [FullPath](../../aspose.zip.xar/xarentry/fullpath/) { get; } | Получает полный путь к записи внутри архива. |
| [IsDirectory](../../aspose.zip.xar/xarentry/isdirectory/) { get; } | Возвращает значение, указывающее, является ли запись каталогом. |
| [LastAccessTime](../../aspose.zip.xar/xarentry/lastaccesstime/) { get; } | Получает время последнего доступа к файлу или каталогу. |
| [ModificationTime](../../aspose.zip.xar/xarentry/modificationtime/) { get; } | Получает время изменения файла или каталога. |
| [Name](../../aspose.zip.xar/xarentry/name/) { get; } | Возвращает имя записи в архиве. |
| [Parent](../../aspose.zip.xar/xarentry/parent/) { get; } | Получает родительский каталог, к которому относится запись. |

## Методы

| Имя | Описание |
| --- | --- |
| [ExtractToDirectory](../../aspose.zip.xar/xardirectoryentry/extracttodirectory/)(string) | Извлекает все файлы из текущего каталога в указанный каталог. |
| override [ToString](../../aspose.zip.xar/xarentry/tostring/)() |  |

### См. также

* class [XarEntry](../xarentry/)
* namespace [Aspose.Zip.Xar](../../aspose.zip.xar/)
* assembly [Aspose.Zip](../../)


