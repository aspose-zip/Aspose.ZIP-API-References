---
title: "LzxArchive.LzxArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор LzxArchive. Инициализирует новый экземпляр класса LzxArchive и формирует список записей, которые можно извлечь из архива."
type: docs
weight: 10
url: /ru/net/aspose.zip.lzx/lzxarchive/lzxarchive/
---
## LzxArchive(Stream, LzxLoadOptions) {#constructor}

Инициализирует новый экземпляр класса [`LzxArchive`](../) и формирует список записей, которые можно извлечь из архива.

```csharp
public LzxArchive(Stream extractionSource, LzxLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| extractionSource | Stream | Источник архива. |
| loadOptions | LzxLoadOptions | Параметры загрузки существующего архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *extractionSource* равен null. |
| ArgumentException | *extractionSource* не поддерживает перемещение. |
| InvalidDataException | Неправильная сигнатура архива. — или — Файл не является архивом LZX. |
| NotImplementedException | Архив Lzx содержит объединённые записи. |
| EndOfStreamException | Поток *extractionSource* слишком короткий. |
| ObjectDisposedException | Выбрасывается, если поток был закрыт. |
| IOException | Произошла ошибка ввода/вывода. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`Extract`](../../lzxarchiveentry/extract/) для распаковки.

### См. также

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzxArchive(string, LzxLoadOptions) {#constructor_1}

Инициализирует новый экземпляр класса [`LzxArchive`](../) и формирует список записей, которые можно извлечь из архива.

```csharp
public LzxArchive(string path, LzxLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Полный или относительный путь к файлу архива. |
| loadOptions | LzxLoadOptions | Параметры загрузки существующего архива. |

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
| InvalidDataException | Файл повреждён. |
| NotImplementedException | Архив Lzx содержит объединённые записи. |
| EndOfStreamException | Файл слишком короткий. |
| ObjectDisposedException | Выбрасывается, если поток был закрыт. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`Extract`](../../lzxarchiveentry/extract/) для распаковки.

## Примеры

В следующем примере архив извлекается, затем первая запись распаковывается в `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (LzxArchive archive = new LzxArchive("sample.lzx"))
{
    archive.Entries[0].Extract(extracted);
}
```

### См. также

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)


