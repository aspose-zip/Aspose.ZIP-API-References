---
title: "LzipArchive.LzipArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор LzipArchive. Инициализирует новый экземпляр LzipArchive"
type: docs
weight: 10
url: /ru/net/aspose.zip.lzip/lziparchive/lziparchive/
---
## LzipArchive(LzipArchiveSettings) {#constructor}

Инициализирует новый экземпляр [`LzipArchive`](../).

```csharp
public LzipArchive(LzipArchiveSettings settings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| настройки | LzipArchiveSettings | Настройка конкретного lzip‑архива с определением размера словаря. |

### См. также

* class [LzipArchiveSettings](../../lziparchivesettings/)
* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

---

## LzipArchive(Stream, LzipLoadOptions) {#constructor_1}

Инициализирует новый экземпляр класса [`LzipArchive`](../), подготовленного для распаковки.

```csharp
public LzipArchive(Stream sourceStream, LzipLoadOptions options = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. |
| параметры | LzipLoadOptions | Параметры для загрузки архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *sourceStream* не поддерживает перемещение. |
| ArgumentNullException | *sourceStream* имеет значение null. |
| InvalidDataException | Заголовки не соответствуют типу lzip‑архива. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |
| IOException | Произошла ошибка ввода/вывода. |

## Примечания

Этот конструктор не распаковывает. См. метод [`Extract`](../extract/) для распаковки.

### См. также

* class [LzipLoadOptions](../../lziploadoptions/)
* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

---

## LzipArchive(string, LzipLoadOptions) {#constructor_2}

Инициализирует новый экземпляр класса [`LzipArchive`](../), подготовленного для распаковки.

```csharp
public LzipArchive(string path, LzipLoadOptions options = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к источнику архива. |
| параметры | LzipLoadOptions | Параметры для загрузки архива. |

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
| InvalidDataException | Заголовки не соответствуют типу lzip‑архива. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |

## Примечания

Этот конструктор не распаковывает. См. метод [`Extract`](../extract/) для распаковки.

## Примеры

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzipArchive(sourceLzipFile))
    {
         archive.Extract(extractedFile);
       }
   }
```

### См. также

* class [LzipLoadOptions](../../lziploadoptions/)
* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)


