---
title: SevenZipArchiveEntry.Extract
second_title: Aspose.ZIP для справочника API .NET
description: SevenZipArchiveEntry метод. Извлекает запись в файловую систему по указанному пути.
type: docs
weight: 80
url: /ru/net/aspose.zip.sevenzip/sevenziparchiveentry/extract/
---
## Extract(string, string) {#extract}

Извлекает запись в файловую систему по указанному пути.

```csharp
public FileInfo Extract(string path, string password = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу назначения. Если файл уже существует, он будет перезаписан. |
| password | String | Необязательный пароль для расшифровки. |

### Возвращаемое значение

Информация о файле составленного файла.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* нулевой. |
| SecurityException | У вызывающего абонента нет необходимого разрешения на доступ. |
| ArgumentException | *path* пуст, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу*path* отказано. |
| PathTooLongException | Указанный*path*, имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. |
| NotSupportedException | Файл в*path* содержит двоеточие (:) в середине строки. |

### Примеры

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Смотрите также

* class [SevenZipArchiveEntry](../)
* пространство имен [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* сборка [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

Извлекает запись в предоставленный поток.

```csharp
public void Extract(Stream destination, string password = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destination | Stream | Целевой поток. Должен быть доступен для записи. |
| password | String | Необязательный пароль для расшифровки. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *destination* не поддерживает запись. |
| InvalidOperationException | Архив не открывается для извлечения. - или - Эта запись является каталогом. |
| InvalidDataException | Неверные данные в записи. |

### Примеры

Извлеките запись zip-архива с паролем.

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Смотрите также

* class [SevenZipArchiveEntry](../)
* пространство имен [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* сборка [Aspose.Zip](../../../)


