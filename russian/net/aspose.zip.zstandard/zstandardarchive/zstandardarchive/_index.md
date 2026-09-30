---
title: "ZstandardArchive.ZstandardArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор ZstandardArchive. Инициализирует новый экземпляр класса ZstandardArchive, подготовленный для сжатия"
type: docs
weight: 10
url: /ru/net/aspose.zip.zstandard/zstandardarchive/zstandardarchive/
---
## ZstandardArchive() {#constructor}

Инициализирует новый экземпляр класса [`ZstandardArchive`](../), подготовленный для сжатия.

```csharp
public ZstandardArchive()
```

## Примеры

В следующем примере показано, как сжать файл.

```csharp
using (ZstandardArchive archive = new ZstandardArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.zst");
}
```

### См. также

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(Stream, ZstandardLoadOptions) {#constructor_1}

Инициализирует новый экземпляр класса [`ZstandardArchive`](../), подготовленный для распаковки.

```csharp
public ZstandardArchive(Stream sourceStream, ZstandardLoadOptions options = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. |
| параметры | ZstandardLoadOptions | Параметры загрузки архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается неожиданно. |
| IOException | Произошла ошибка ввода/вывода. |
| InvalidDataException | Выбрасывается, когда данные недействительны или повреждены. |

## Примечания

Этот конструктор не выполняет распаковку. См. метод [`Open`](../open/) для распаковки.

## Примеры

Откройте архив из потока и извлеките его в `MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new ZstandardArchive(File.OpenRead("archive.zst")))
  archive.Open().CopyTo(ms);
```

### См. также

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(string, ZstandardLoadOptions) {#constructor_2}

Инициализирует новый экземпляр класса [`ZstandardArchive`](../).

```csharp
public ZstandardArchive(string path, ZstandardLoadOptions options = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу архива. |
| параметры | ZstandardLoadOptions | Параметры загрузки архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* имеет значение null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | *path* пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *path* запрещён. |
| PathTooLongException | Указанный *path*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл по адресу *path* содержит двоеточие (:) в середине строки. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается неожиданно. |
| FileNotFoundException | Файл не найден. |
| IOException | Файл уже открыт. |
| InvalidDataException | Выбрасывается, когда данные недействительны или повреждены. |

## Примечания

Этот конструктор не выполняет распаковку. См. метод [`Open`](../open/) для распаковки.

## Примеры

Откройте архив из файла по пути и извлеките его в `MemoryStream`

```csharp
var ms = new MemoryStream();
using (ZstandardArchive archive = new ZstandardArchive("archive.zst"))
  archive.Open().CopyTo(ms);
```

### См. также

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


