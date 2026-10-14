---
title: "RarArchiveEntry.Extract"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "RarArchiveEntry метод. Извлекает элемент в файловую систему по указанному пути"
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
| path | String | Путь к целевому файлу. Если файл уже существует, он будет перезаписан. |
| password | String | Необязательный пароль для расшифровки. |

### Возвращаемое значение

Информация о составленном файле.

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
| InvalidDataException | Данные повреждены. -или- проверка CRC или MAC для элемента не удалась. |
| OperationCanceledException | В .NET Framework 4.0 и выше: Выбрасывается, когда извлечение отменяется с помощью предоставленного токена отмены. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |

## Примеры

Извлечь две записи из rar-архива.

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

### См. также

* class [RarArchiveEntry](../)
* namespace [Aspose.Zip.Rar](../../rararchiveentry/)
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
| InvalidDataException | Проверка CRC или MAC для элемента не удалась. |
| ArgumentException | *destination* не поддерживает запись. |
| InvalidDataException | Данные повреждены. -или- проверка CRC или MAC для элемента не удалась. |
| OperationCanceledException | В .NET Framework 4.0 и выше: Выбрасывается, когда извлечение отменяется с помощью предоставленного токена отмены. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |

## Примеры

Извлеките элемент rar‑архива с паролем.

```csharp
using (FileStream rarFile = File.Open("archive.zip", FileMode.Open))
{
    using (RarArchive archive = new RarArchive(rarFile))
    {
        archive.Entries[0].Extract(httpResponseStream, "p@s$");
    }
}
```

### См. также

* class [RarArchiveEntry](../)
* namespace [Aspose.Zip.Rar](../../rararchiveentry/)
* assembly [Aspose.Zip](../../../)


