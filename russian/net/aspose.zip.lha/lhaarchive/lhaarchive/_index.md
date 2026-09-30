---
title: "LhaArchive.LhaArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор LhaArchive. Инициализирует новый экземпляр класса LhaArchive и формирует список записей, которые можно извлечь из архива"
type: docs
weight: 10
url: /ru/net/aspose.zip.lha/lhaarchive/lhaarchive/
---
## LhaArchive(Stream, LhaLoadOptions) {#constructor}

Инициализирует новый экземпляр класса [`LhaArchive`](../) и формирует список записей, которые можно извлечь из архива.

```csharp
public LhaArchive(Stream sourceStream, LhaLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. |
| loadOptions | LhaLoadOptions | Параметры загрузки существующего архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *sourceStream* равен null |
| ArgumentException | *sourceStream* не поддерживает перемотку. |
| InvalidDataException | Обнаружены неподходящие данные. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| ObjectDisposedException | Выбрасывается, когда объект был освобождён. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`Extract`](../../lhaarchiveentry/extract/) для распаковки.

### См. также

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LhaArchive(string, LhaLoadOptions) {#constructor_1}

Инициализирует новый экземпляр класса [`LhaArchive`](../) и формирует список записей, которые можно извлечь из архива.

```csharp
public LhaArchive(string path, LhaLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Полный или относительный путь к файлу архива. |
| loadOptions | LhaLoadOptions | Параметры загрузки существующего архива. |

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
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| ObjectDisposedException | Выбрасывается, когда объект был освобождён. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`Extract`](../../lhaarchiveentry/extract/) для распаковки.

## Примеры

В следующем примере архив извлекается, затем первая запись распаковывается в `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (LhaArchive archive = new LhaArchive("sample.lzh"))
{
    archive.Entries[0].Extract(extracted);
}
```

### См. также

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)


