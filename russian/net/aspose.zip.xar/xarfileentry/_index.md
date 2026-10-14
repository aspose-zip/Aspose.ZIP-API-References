---
title: "Класс XarFileEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Xar.XarFileEntry. Представляет запись файла внутри архива xar."
type: docs
weight: 1470
url: /ru/net/aspose.zip.xar/xarfileentry/
---
## XarFileEntry class

Представляет файловую запись внутри архива xar.

```csharp
public sealed class XarFileEntry : XarEntry, IArchiveFileEntry
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CreationTime](../../aspose.zip.xar/xarentry/creationtime/) { get; } | Получает время создания файла или каталога. |
| [FullPath](../../aspose.zip.xar/xarentry/fullpath/) { get; } | Получает полный путь к записи внутри архива. |
| [IsDirectory](../../aspose.zip.xar/xarentry/isdirectory/) { get; } | Возвращает значение, указывающее, является ли запись каталогом. |
| [LastAccessTime](../../aspose.zip.xar/xarentry/lastaccesstime/) { get; } | Получает время последнего доступа к файлу или каталогу. |
| [Length](../../aspose.zip.xar/xarfileentry/length/) { get; } | Получает длину записи в байтах. |
| [ModificationTime](../../aspose.zip.xar/xarentry/modificationtime/) { get; } | Получает время изменения файла или каталога. |
| [Name](../../aspose.zip.xar/xarentry/name/) { get; } | Возвращает имя записи в архиве. |
| [Parent](../../aspose.zip.xar/xarentry/parent/) { get; } | Получает родительский каталог, к которому относится запись. |

## Методы

| Имя | Описание |
| --- | --- |
| [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract_1)(Stream) | Извлекает запись в предоставленный поток. |
| [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract)(string) | Извлекает запись в файловую систему по указанному пути. |
| [Open](../../aspose.zip.xar/xarfileentry/open/)() | Открывает запись для извлечения и предоставляет поток с содержимым записи. |
| override [ToString](../../aspose.zip.xar/xarentry/tostring/)() |  |

## События

| Имя | Описание |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.xar/xarfileentry/compressionprogressed/) | Вызывается, когда часть необработанного потока сжата. |

### См. также

* class [XarEntry](../xarentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Xar](../../aspose.zip.xar/)
* assembly [Aspose.Zip](../../)


