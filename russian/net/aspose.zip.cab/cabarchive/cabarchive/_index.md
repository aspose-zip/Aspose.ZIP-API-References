---
title: "CabArchive.CabArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор CabArchive. Инициализирует новый экземпляр класса CabArchive, подготовленный для сжатия"
type: docs
weight: 10
url: /ru/net/aspose.zip.cab/cabarchive/cabarchive/
---
## CabArchive(CabEntrySettings) {#constructor}

Инициализирует новый экземпляр класса [`CabArchive`](../), подготовленного для сжатия.

```csharp
public CabArchive(CabEntrySettings settings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| settings | CabEntrySettings | Настройки сжатия и шифрования, используемые для недавно добавленных элементов [`CabEntry`](../../cabentry/). Если не указано, будет использовано сжатие MSZIP. |

## Примеры

В следующем примере показано, как сжать файл.

```csharp
using (var archive = new CabArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cab");
}
```

Сжать файл, используя конкретные настройки сжатия.

```csharp
using (var archive = new CabArchive())
{
    var settings = new CabEntrySettings(new CabStoreCompressionSettings());
    archive.CreateEntry("entry.bin", "data.bin", settings);
    archive.Save("archive.cab");
}
```

### См. также

* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CabArchive(Stream, CabLoadOptions) {#constructor_1}

Инициализирует новый экземпляр класса [`CabArchive`](../) и формирует список записей, которые можно извлечь из архива.

```csharp
public CabArchive(Stream sourceStream, CabLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. Должен поддерживать поиск. |
| loadOptions | CabLoadOptions | Параметры загрузки существующего архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *sourceStream* имеет значение null. |
| ArgumentException | *sourceStream* не поддерживает перемещение. |
| InvalidDataException | *sourceStream* не является действительным архивом CAB. |
| EndOfStreamException | Поток слишком короткий. |
| ObjectDisposedException | Выбрасывается, когда поток был освобождён. |
| IOException | Произошла ошибка ввода/вывода. |
| NotSupportedException | Поток не поддерживает перемещение позиции, например, если он построен из канала или вывода консоли. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`Open`](../../cabentry/open/) для распаковки.

## Примеры

В следующем примере показано, как извлечь все записи в каталог.

```csharp
using (var archive = new CabArchive(File.OpenRead("archive.cab")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### См. также

* class [CabLoadOptions](../../cabloadoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CabArchive(string, CabLoadOptions) {#constructor_2}

Инициализирует новый экземпляр класса [`CabArchive`](../) и формирует список записей, которые можно извлечь из архива.

```csharp
public CabArchive(string path, CabLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу архива. |
| loadOptions | CabLoadOptions | Параметры загрузки существующего архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* имеет значение null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | *path* пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *path* запрещён. |
| PathTooLongException | Указанный *path*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл по адресу *path* содержит двоеточие (:) в середине строки. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| FileNotFoundException | Файл не найден. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| IOException | Файл уже открыт. |
| EndOfStreamException | Файл слишком короткий. |
| InvalidDataException | Магическое число CAB недействительно или размер заголовка не совпадает. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`Open`](../../cabentry/open/) для распаковки.

## Примеры

В следующем примере показано, как извлечь все записи в каталог.

```csharp
using (var archive = new CabArchive("archive.cab")) hj
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### См. также

* class [CabLoadOptions](../../cabloadoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


