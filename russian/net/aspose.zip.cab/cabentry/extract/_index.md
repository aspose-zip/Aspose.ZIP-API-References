---
title: Extract
second_title: Aspose.ZIP для справочника API .NET
description: Извлекает запись в файловую систему по указанному пути.
type: docs
weight: 30
url: /ru/net/aspose.zip.cab/cabentry/extract/
---
## Extract(string) {#extract}

Извлекает запись в файловую систему по указанному пути.

```csharp
public FileSystemInfo Extract(string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу назначения. Если файл уже существует, он будет перезаписан. |

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
using (var archive = new CabArchive("archive.cab"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Смотрите также

* class [CabEntry](../../cabentry)
* пространство имен [Aspose.Zip.Cab](../../cabentry)
* сборка [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Извлекает запись в указанный поток.

```csharp
public void Extract(Stream destination)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destination | Stream | Целевой поток. Должен быть доступен для записи. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *destination*не поддерживает запись. |

### Примеры

Извлечь запись из CAB-архива.

```csharp
using (var archive = new CabArchive("archive.cab"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Смотрите также

* class [CabEntry](../../cabentry)
* пространство имен [Aspose.Zip.Cab](../../cabentry)
* сборка [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
