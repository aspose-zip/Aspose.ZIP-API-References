---
title: Extract
second_title: Aspose.ZIP для справочника API .NET
description: Извлекает запись в файловую систему по указанному пути.
type: docs
weight: 60
url: /ru/net/aspose.zip.sevenzip/sevenziparchiveentry/extract/
---
## SevenZipArchiveEntry.Extract method

Извлекает запись в файловую систему по указанному пути.

```csharp
public FileInfo Extract(string path, string password = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу назначения. Если файл уже существует, он будет перезаписан. |
| пароль | String | Необязательный пароль для расшифровки. |

### Возвращаемое значение

Информация о скомпонованном файле.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path*равно null. |
| SecurityException | Вызывающий объект не имеет необходимого разрешения на доступ. |
| ArgumentException | *path*пуст, содержит только пробелы или недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу*path*запрещен. |
| PathTooLongException | Указанный*path*, имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. |
| NotSupportedException | Файл по адресу*path*содержит двоеточие (:) в середине строки. |

### Примеры

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Смотрите также

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* пространство имен [Aspose.Zip.SevenZip](../../sevenziparchiveentry)
* сборка [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->