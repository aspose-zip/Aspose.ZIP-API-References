---
title: ArchiveEntry.Extract
second_title: Aspose.ZIP для справочника API .NET
description: ArchiveEntry метод. Извлекает запись в файловую систему по указанному пути.
type: docs
weight: 100
url: /ru/net/aspose.zip/archiveentry/extract/
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
| InvalidDataException | Ошибка проверки CRC или MAC для записи. |

### Примеры

Извлеките две записи zip-архива, каждая со своим паролем

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Open))
{
    using (Archive archive = new Archive(zipFile))
    {
        archive.Entries[0].Extract("first.bin", "first_pass");
        archive.Entries[1].Extract("second.bin", "second_pass");
    }
}
```

### Смотрите также

* class [ArchiveEntry](../)
* пространство имен [Aspose.Zip](../../archiveentry/)
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
| InvalidDataException | Ошибка проверки CRC или MAC для записи. |
| ArgumentException | *destination* не поддерживает запись. |

### Примеры

Извлеките запись zip-архива с паролем.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Open))
{
    using (Archive archive = new Archive(zipFile))
    {
        archive.Entries[0].Extract(httpResponseStream, "p@s$");
    }
}
```

### Смотрите также

* class [ArchiveEntry](../)
* пространство имен [Aspose.Zip](../../archiveentry/)
* сборка [Aspose.Zip](../../../)


