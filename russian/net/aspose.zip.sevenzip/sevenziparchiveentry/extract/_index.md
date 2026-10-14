---
title: "SevenZipArchiveEntry.Extract"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод SevenZipArchiveEntry. Извлекает запись в файловую систему по указанному пути"
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
| path | String | Путь к целевому файлу. Если файл уже существует, он будет перезаписан. |
| password | String | Необязательный пароль для расшифровки. |

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
| InvalidDataException | Архив повреждён. |
| OperationCanceledException | В .NET Framework 4.0 и выше: Выбрасывается, когда извлечение отменяется с помощью предоставленного токена отмены. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |
| FileNotFoundException | Файл не найден. |

## Примеры

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### См. также

* class [SevenZipArchiveEntry](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

Извлекает запись в предоставленный поток.

```csharp
public void Extract(Stream destination, string password = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | Stream | Поток назначения. Должен поддерживать запись. |
| password | String | Необязательный пароль для расшифровки. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *destination* не поддерживает запись. |
| InvalidOperationException | Архив не открыт для извлечения. - или - Эта запись является каталогом. |
| InvalidDataException | Неправильные данные в записи. |
| OperationCanceledException | В .NET Framework 4.0 и выше: Выбрасывается, когда извлечение отменяется с помощью предоставленного токена отмены. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |

## Примеры

Извлеките элемент zip‑архива с паролем.

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### См. также

* class [SevenZipArchiveEntry](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* assembly [Aspose.Zip](../../../)


