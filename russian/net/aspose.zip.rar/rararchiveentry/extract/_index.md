---
title: Extract
second_title: Aspose.ZIP для справочника API .NET
description: Извлекает запись в файловую систему по указанному пути.
type: docs
weight: 90
url: /ru/net/aspose.zip.rar/rararchiveentry/extract/
---
## Extract(string, string) {#extract}

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
| SecurityException | У вызывающего абонента нет необходимых прав доступа для доступа |
| ArgumentException | *path*пуст, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу*path*запрещен. |
| PathTooLongException | Указанный*path*, имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. |
| NotSupportedException | Файл по адресу*path*содержит двоеточие (:) в середине строки. |
| InvalidDataException | Проверка CRC или MAC для записи не удалась. |

### Примеры

Извлечь две записи из архива rar.

```csharp
using (FileStream rarFile = File.Open("archive.rar", FileMode.Open))
{
    using (RarArchive archive = new RarArchive(rarFile))
    {
        archive.Entries[0].Extract("first.bin", "pass");
        archive.Entries[1].Extract("second.bin", "pass");
    }
}
```

### Смотрите также

* class [RarArchiveEntry](../../rararchiveentry)
* пространство имен [Aspose.Zip.Rar](../../rararchiveentry)
* сборка [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

Извлекает запись в указанный поток.

```csharp
public void Extract(Stream destination, string password = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destination | Stream | Целевой поток. Должен быть доступен для записи. |
| пароль | String | Необязательный пароль для расшифровки. |

### Исключения

| исключение | условие |
| --- | --- |
| InvalidDataException | Проверка CRC или MAC для записи не удалась. |
| ArgumentException | *destination*не поддерживает запись. |

### Примеры

Извлечь запись из архива rar с паролем.

```csharp
using (FileStream rarFile = File.Open("archive.zip", FileMode.Open))
{
    using (RarArchive archive = new RarArchive(rarFile))
    {
        archive.Entries[0].Extract(httpResponseStream, "p@s$");
    }
}
```

### Смотрите также

* class [RarArchiveEntry](../../rararchiveentry)
* пространство имен [Aspose.Zip.Rar](../../rararchiveentry)
* сборка [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->