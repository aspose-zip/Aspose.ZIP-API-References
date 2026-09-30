---
title: "RarArchive.RarArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор RarArchive. Инициализирует новый экземпляр класса RarArchive и формирует список записей, которые можно извлечь из архива"
type: docs
weight: 10
url: /ru/net/aspose.zip.rar/rararchive/rararchive/
---
## RarArchive(string, RarArchiveLoadOptions) {#constructor_1}

Инициализирует новый экземпляр класса [`RarArchive`](../) и формирует список записей, которые можно извлечь из архива.

```csharp
public RarArchive(string path, RarArchiveLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Полный или относительный путь к файлу архива. |
| loadOptions | RarArchiveLoadOptions | Параметры загрузки существующего архива. |

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
| InvalidDataException | Выбрасывается, когда данные недействительны или повреждены. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`Open`](../../rararchiveentry/open/) для распаковки.

## Примеры

В следующем примере архив извлекается, затем первая запись распаковывается в `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive("data.rar"))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### См. также

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* namespace [Aspose.Zip.Rar](../../rararchive/)
* assembly [Aspose.Zip](../../../)

---

## RarArchive(Stream, RarArchiveLoadOptions) {#constructor}

Инициализирует новый экземпляр класса [`RarArchive`](../) и формирует список записей, которые можно извлечь из архива.

```csharp
public RarArchive(Stream sourceStream, RarArchiveLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. |
| loadOptions | RarArchiveLoadOptions | Параметры загрузки существующего архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *sourceStream* не поддерживает перемещение. |
| InvalidDataException | Неверная сигнатура архива. – или – Файл не является RAR‑архивом. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`Open`](../../rararchiveentry/open/) для распаковки.

## Примеры

В следующем примере происходит расшифровка и распаковка первой записи в `MemoryStream`.

```csharp
var fs = File.OpenRead("encrypted.rar");
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive(fs, new RarArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### См. также

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* namespace [Aspose.Zip.Rar](../../rararchive/)
* assembly [Aspose.Zip](../../../)


