---
title: "WimArchive.WimArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор WimArchive. Инициализирует новый экземпляр класса WimArchive и формирует список записей, которые могут быть извлечены из архива"
type: docs
weight: 10
url: /ru/net/aspose.zip.wim/wimarchive/wimarchive/
---
## WimArchive(Stream, WimLoadOptions) {#constructor}

Инициализирует новый экземпляр класса [`WimArchive`](../) и формирует список записей, которые могут быть извлечены из архива.

```csharp
public WimArchive(Stream sourceStream, WimLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. Должен поддерживать поиск. |
| loadOptions | WimLoadOptions | Параметры загрузки существующего архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *sourceStream* имеет значение null. |
| ArgumentException | *sourceStream* не поддерживает перемещение. |
| InvalidDataException | *sourceStream* не является действительным wim-архивом. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |
| NotSupportedException | Заголовок указывает на многотомный архив. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`Open`](../../wimfileentry/open/) для распаковки.

## Примеры

В следующем примере показано, как извлечь все записи в каталог.

```csharp
using (var archive = new WimArchive(File.OpenRead("archive.wim")))
{ 
   archive.Images[0].ExtractToDirectory("C:\\extracted");
}
```

### См. также

* class [WimLoadOptions](../../wimloadoptions/)
* class [WimArchive](../)
* namespace [Aspose.Zip.Wim](../../wimarchive/)
* assembly [Aspose.Zip](../../../)

---

## WimArchive(string, WimLoadOptions) {#constructor_1}

Инициализирует новый экземпляр класса [`WimArchive`](../) и формирует список записей, которые могут быть извлечены из архива.

```csharp
public WimArchive(string path, WimLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу архива. |
| loadOptions | WimLoadOptions | Параметры загрузки существующего архива. |

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
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| InvalidDataException | Заголовок указывает на многотомный архив. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`Open`](../../wimfileentry/open/) для распаковки.

## Примеры

В следующем примере показано, как извлечь все записи в каталог.

```csharp
using (var archive = new WimArchive("archive.wim")) 
{ 
   archive.Images[0].ExtractToDirectory("C:\\extracted");
}
```

### См. также

* class [WimLoadOptions](../../wimloadoptions/)
* class [WimArchive](../)
* namespace [Aspose.Zip.Wim](../../wimarchive/)
* assembly [Aspose.Zip](../../../)


