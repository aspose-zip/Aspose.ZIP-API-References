---
title: RarArchiveEntry.Extract
second_title: Aspose.ZIP для справочника API .NET
description: RarArchiveEntry метод. Извлекает запись в файловую систему по указанному пути.
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

Извлеките две записи архива rar.

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

* class [RarArchiveEntry](../)
* пространство имен [Aspose.Zip.Rar](../../rararchiveentry/)
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

* class [RarArchiveEntry](../)
* пространство имен [Aspose.Zip.Rar](../../rararchiveentry/)
* сборка [Aspose.Zip](../../../)


