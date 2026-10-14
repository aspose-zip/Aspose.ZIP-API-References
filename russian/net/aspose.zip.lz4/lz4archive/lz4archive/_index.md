---
title: "Lz4Archive.Lz4Archive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор Lz4Archive. Инициализирует новый экземпляр класса Lz4Archive, подготовленный для распаковки"
type: docs
weight: 10
url: /ru/net/aspose.zip.lz4/lz4archive/lz4archive/
---
## Lz4Archive(Stream, Lz4LoadOptions) {#constructor_1}

Инициализирует новый экземпляр класса [`Lz4Archive`](../), подготовленного для распаковки.

```csharp
public Lz4Archive(Stream sourceStream, Lz4LoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. |
| loadOptions | Lz4LoadOptions | Параметры загрузки архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | Не удалось прочитать из *sourceStream* |
| ArgumentNullException | *sourceStream* имеет значение null. |
| EndOfStreamException | *sourceStream* слишком короток. |
| InvalidDataException | *sourceStream* имеет неверную сигнатуру. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |
| IOException | Произошла ошибка ввода/вывода. |

## Примечания

Этот конструктор не выполняет распаковку. См. метод [`Open`](../open/) для распаковки.

## Примеры

Откройте архив из потока и извлеките его в `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive(File.OpenRead("archive.lz4")))
  archive.Open().CopyTo(ms);
```

### См. также

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(string, Lz4LoadOptions) {#constructor_2}

Инициализирует новый экземпляр класса [`Lz4Archive`](../).

```csharp
public Lz4Archive(string path, Lz4LoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу архива. |
| loadOptions | Lz4LoadOptions | Параметры загрузки архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* имеет значение null. |
| SecurityException | Вызвавший процесс не имеет необходимого разрешения для доступа. |
| ArgumentException | *path* пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *path* запрещён. |
| PathTooLongException | Указанный *path*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл по адресу *path* содержит двоеточие (:) в середине строки. |
| EndOfStreamException | Файл слишком короткий. |
| InvalidDataException | Данные в файле имеют неверную сигнатуру. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| FileNotFoundException | Файл не найден. |
| IOException | Файл уже открыт. |

## Примечания

Этот конструктор не выполняет распаковку. См. метод [`Open`](../open/) для распаковки.

## Примеры

Откройте архив из файла по пути и извлеките его в `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive("archive.lz4"))
  archive.Open().CopyTo(ms);
```

### См. также

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(Lz4ArchiveSetting) {#constructor}

Инициализирует новый экземпляр класса [`Lz4Archive`](../), подготовленного для сжатия.

```csharp
public Lz4Archive(Lz4ArchiveSetting settings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| настройки | Lz4ArchiveSetting | Настройка составного архива. |

### См. также

* class [Lz4ArchiveSetting](../../lz4archivesetting/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


