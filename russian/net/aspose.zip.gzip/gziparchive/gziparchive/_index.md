---
title: "GzipArchive.GzipArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор GzipArchive. Инициализирует новый экземпляр класса GzipArchive, подготовленный для сжатия"
type: docs
weight: 10
url: /ru/net/aspose.zip.gzip/gziparchive/gziparchive/
---
## GzipArchive() {#constructor}

Инициализирует новый экземпляр класса [`GzipArchive`](../), подготовленного для сжатия.

```csharp
public GzipArchive()
```

## Примеры

В следующем примере показано, как сжать файл.

```csharp
using (GzipArchive archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### См. также

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## GzipArchive(Stream, bool) {#constructor_2}

Инициализирует новый экземпляр класса [`GzipArchive`](../), подготовленного для распаковки.

```csharp
public GzipArchive(Stream sourceStream, bool parseHeader = false)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. |
| parseHeader | Boolean | Определяет, следует ли разбирать заголовок потока, чтобы определить свойства, включая имя. Имеет смысл только для потоков, поддерживающих перемещение. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *sourceStream* имеет значение null. |
| EndOfStreamException | *sourceStream* слишком короток. |
| InvalidDataException | *sourceStream* имеет неверную сигнатуру. |

## Примечания

Этот конструктор не выполняет распаковку. См. метод [`Open`](../open/) для распаковки.

## Примеры

Откройте архив из потока и извлеките его в `MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive(File.OpenRead("archive.gz")))
  archive.Open().CopyTo(ms);
```

### См. также

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## GzipArchive(Stream, GzipLoadOptions) {#constructor_1}

Инициализирует новый экземпляр класса [`GzipArchive`](../), подготовленного для распаковки.

```csharp
public GzipArchive(Stream sourceStream, GzipLoadOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. |
| параметры | GzipLoadOptions | Параметры для загрузки архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *sourceStream* имеет значение null. |
| EndOfStreamException | *sourceStream* слишком короток. |
| InvalidDataException | *sourceStream* имеет неверную сигнатуру. |

## Примечания

Этот конструктор не выполняет распаковку. См. метод [`Open`](../open/) для распаковки.

## Примеры

Откройте архив из потока и извлеките его в `MemoryStream`

```csharp
var ms = new MemoryStream();
GzipLoadOptions options = new GzipLoadOptions();
using (GzipArchive archive = new GzipArchive(File.OpenRead("archive.gz"), options))
  archive.Extract(ms);
```

### См. также

* class [GzipLoadOptions](../../gziploadoptions/)
* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## GzipArchive(string, GzipLoadOptions) {#constructor_3}

Инициализирует новый экземпляр класса [`GzipArchive`](../), подготовленного для распаковки.

```csharp
public GzipArchive(string path, GzipLoadOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу архива. |
| параметры | GzipLoadOptions | Параметры для загрузки архива. |

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

## Примечания

Этот конструктор не выполняет распаковку. См. метод [`Open`](../open/) для распаковки.

## Примеры

Откройте архив из файла по пути и извлеките его в `MemoryStream`

```csharp
var ms = new MemoryStream();
GzipLoadOptions options = new GzipLoadOptions();
using (GzipArchive archive = new GzipArchive("archive.gz", options))
  archive.Extract(ms);
```

### См. также

* class [GzipLoadOptions](../../gziploadoptions/)
* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## GzipArchive(string, bool) {#constructor_4}

Инициализирует новый экземпляр класса [`GzipArchive`](../), подготовленного для распаковки.

```csharp
public GzipArchive(string path, bool parseHeader = false)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу архива. |
| parseHeader | Boolean | Определяет, следует ли разбирать заголовок потока, чтобы определить свойства, включая имя. Имеет смысл только для потоков, поддерживающих перемещение. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* имеет значение null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | *path* пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *path* запрещён. |
| PathTooLongException | Указанный *path*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл по адресу *path* содержит двоеточие (:) в середине строки. |
| EndOfStreamException | Файл слишком короткий. |
| InvalidDataException | Данные в файле имеют неверную сигнатуру. |

## Примечания

Этот конструктор не выполняет распаковку. См. метод [`Open`](../open/) для распаковки.

## Примеры

Откройте архив из файла по пути и извлеките его в `MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive("archive.gz"))
  archive.Open().CopyTo(ms);
```

### См. также

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


