---
title: "CabEntry.Extract"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод CabEntry. Извлекает запись в файловую систему по указанному пути"
type: docs
weight: 40
url: /ru/net/aspose.zip.cab/cabentry/extract/
---
## Extract(string) {#extract}

Извлекает запись в файловую систему по указанному пути.

```csharp
public FileInfo Extract(string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к целевому файлу. Если файл уже существует, он будет перезаписан. |

### Возвращаемое значение

Информация о файле составного файла.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* имеет значение null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | *path* пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *path* запрещён. |
| PathTooLongException | Указанный *path*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл по адресу *path* содержит двоеточие (:) в середине строки. |
| FileNotFoundException | Файл не найден. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| IOException | Файл уже открыт. |
| NotSupportedException | Инициализация потока не удалась из‑за неверных данных. |
| InvalidDataException | Архив повреждён. |
| OperationCanceledException | В .NET Framework 4.0 и выше: Выбрасывается, когда извлечение отменяется с помощью предоставленного токена отмены. |
| InvalidOperationException | Запись принадлежит архиву, подготовленному для компоновки. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |

## Примеры

```csharp
using (var archive = new CabArchive("archive.cab"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### См. также

* class [CabEntry](../)
* namespace [Aspose.Zip.Cab](../../cabentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Извлекает запись в предоставленный поток.

```csharp
public void Extract(Stream destination)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | Stream | Поток назначения. Должен поддерживать запись. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *destination* не поддерживает запись. |
| NotSupportedException | Инициализация потока не удалась из‑за неверных данных. |
| InvalidDataException | Архив повреждён. |
| OperationCanceledException | В .NET Framework 4.0 и выше: Выбрасывается, когда извлечение отменяется с помощью предоставленного токена отмены. |
| InvalidOperationException | Запись принадлежит архиву, подготовленному для компоновки. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |

## Примеры

Извлечь запись из CAB‑архива.

```csharp
using (var archive = new CabArchive("archive.cab"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### См. также

* class [CabEntry](../)
* namespace [Aspose.Zip.Cab](../../cabentry/)
* assembly [Aspose.Zip](../../../)


