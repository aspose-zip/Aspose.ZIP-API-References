---
title: TarEntry.Extract
second_title: Aspose.ZIP для справочника API .NET
description: TarEntry метод. Извлекает запись в файловую систему по указанному пути.
type: docs
weight: 40
url: /ru/net/aspose.zip.tar/tarentry/extract/
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
using (var archive = new TarArchive("archive.tar"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Смотрите также

* class [TarEntry](../)
* пространство имен [Aspose.Zip.Tar](../../tarentry/)
* сборка [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Извлекает запись в предоставленный поток.

```csharp
public void Extract(Stream destination)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destination | Stream | Целевой поток. Должен быть доступен для записи. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *destination* не поддерживает запись. |

### Примеры

Извлеките запись из архива tar.

```csharp
using (var archive = new TarArchive("archive.tar"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Смотрите также

* class [TarEntry](../)
* пространство имен [Aspose.Zip.Tar](../../tarentry/)
* сборка [Aspose.Zip](../../../)


