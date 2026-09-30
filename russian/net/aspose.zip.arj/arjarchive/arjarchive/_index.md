---
title: "ArjArchive.ArjArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор ArjArchive. Инициализирует новый экземпляр класса ArjArchive и формирует список записей, которые могут быть извлечены из архива."
type: docs
weight: 10
url: /ru/net/aspose.zip.arj/arjarchive/arjarchive/
---
## ArjArchive(Stream, ArjLoadOptions) {#constructor}

Инициализирует новый экземпляр класса [`ArjArchive`](../) и формирует список записей, которые могут быть извлечены из архива.

```csharp
public ArjArchive(Stream extractionSource, ArjLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| extractionSource | Stream | Источник архива. |
| loadOptions | ArjLoadOptions | Параметры загрузки существующего архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *extractionSource* равен null. |
| ArgumentException | &gt;*extractionSource* не поддерживает перемещение. |
| InvalidDataException | Неверная подпись архива. - или - Файл не является ARJ-архивом. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до того, как все байты заголовка или имени были прочитаны. |
| NotSupportedException | Архив повреждён. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`Extract`](../../arjentryplain/extract/) для распаковки.

### См. также

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)

---

## ArjArchive(string, ArjLoadOptions) {#constructor_1}

Инициализирует новый экземпляр класса [`ArjArchive`](../) и формирует список записей, которые могут быть извлечены из архива.

```csharp
public ArjArchive(string path, ArjLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу архива. |
| loadOptions | ArjLoadOptions | Параметры загрузки существующего архива. |

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
| EndOfStreamException | Выбрасывается, когда конец потока достигается до того, как все байты заголовка или имени были прочитаны. |
| InvalidDataException | Магическое число ARJ недействительно или размер заголовка выходит за пределы допустимого. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`Extract`](../../arjentryplain/extract/) для распаковки.

## Примеры

В следующем примере показано, как извлечь все записи в каталог.

```csharp
using (var archive = new ArjArchive("archive.arj")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### См. также

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


