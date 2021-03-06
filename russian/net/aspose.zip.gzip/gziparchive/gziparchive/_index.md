---
title: GzipArchive
second_title: Aspose.ZIP для справочника API .NET
description: Инициализирует новый экземпляр классаGzipArchiveaspose.zip.gzip/gziparchive подготовленный для сжатия.
type: docs
weight: 10
url: /ru/net/aspose.zip.gzip/gziparchive/gziparchive/
---
## GzipArchive() {#constructor}

Инициализирует новый экземпляр класса[`GzipArchive`](../../gziparchive), подготовленный для сжатия.

```csharp
public GzipArchive()
```

### Примеры

В следующем примере показано, как сжать файл.

```csharp
using (GzipArchive archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### Смотрите также

* class [GzipArchive](../../gziparchive)
* пространство имен [Aspose.Zip.Gzip](../../gziparchive)
* сборка [Aspose.Zip](../../../)

---

## GzipArchive(Stream, bool) {#constructor_1}

Инициализирует новый экземпляр класса[`GzipArchive`](../../gziparchive), подготовленный для распаковки.

```csharp
public GzipArchive(Stream sourceStream, bool parseHeader = false)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. |
| parseHeader | Boolean | Следует ли анализировать заголовок потока для определения свойств, включая имя. Имеет смысл только для потока с возможностью поиска. |

### Примечания

Этот конструктор не распаковывается. См.[`Open`](../open)метод распаковки.

### Примеры

Открыть архив из потока и извлечь его в` MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive(File.OpenRead("archive.gz")))
  archive.Open().CopyTo(ms);
```

### Смотрите также

* class [GzipArchive](../../gziparchive)
* пространство имен [Aspose.Zip.Gzip](../../gziparchive)
* сборка [Aspose.Zip](../../../)

---

## GzipArchive(string, bool) {#constructor_2}

Инициализирует новый экземпляр класса[`GzipArchive`](../../gziparchive).

```csharp
public GzipArchive(string path, bool parseHeader = false)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу архива. |
| parseHeader | Boolean | Следует ли анализировать заголовок потока для определения свойств, включая имя. Имеет смысл только для потока с возможностью поиска. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path*равно null. |
| SecurityException | У вызывающего абонента нет необходимых прав доступа для доступа |
| ArgumentException | *path*пуст, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу*path*запрещен. |
| PathTooLongException | Указанный*path*, имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. |
| NotSupportedException | Файл по адресу*path*содержит двоеточие (:) в середине строки. |

### Примечания

Этот конструктор не распаковывается. См.[`Open`](../open)метод распаковки.

### Примеры

Открыть архив из файла по пути и распаковать его в` MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive("archive.gz"))
  archive.Open().CopyTo(ms);
```

### Смотрите также

* class [GzipArchive](../../gziparchive)
* пространство имен [Aspose.Zip.Gzip](../../gziparchive)
* сборка [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
