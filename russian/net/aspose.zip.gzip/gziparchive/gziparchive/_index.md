---
title: GzipArchive.GzipArchive
second_title: Aspose.ZIP для справочника API .NET
description: GzipArchive строитель. Инициализирует новый экземплярGzipArchive класс подготовлен к сжатию.
type: docs
weight: 10
url: /ru/net/aspose.zip.gzip/gziparchive/gziparchive/
---
## GzipArchive() {#constructor}

Инициализирует новый экземпляр[`GzipArchive`](../) класс подготовлен к сжатию.

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

* class [GzipArchive](../)
* пространство имен [Aspose.Zip.Gzip](../../gziparchive/)
* сборка [Aspose.Zip](../../../)

---

## GzipArchive(Stream, bool) {#constructor_1}

Инициализирует новый экземпляр[`GzipArchive`](../) класс подготовлен к распаковке.

```csharp
public GzipArchive(Stream sourceStream, bool parseHeader = false)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. |
| parseHeader | Boolean | Следует ли анализировать заголовок потока, чтобы выяснить свойства, включая имя. Имеет смысл только для потока с возможностью поиска. |

### Примечания

Этот конструктор не распаковывается. Видеть[`Open`](../open/) метод распаковки.

### Примеры

Откройте архив из потока и распакуйте его в`ПамятьПоток`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive(File.OpenRead("archive.gz")))
  archive.Open().CopyTo(ms);
```

### Смотрите также

* class [GzipArchive](../)
* пространство имен [Aspose.Zip.Gzip](../../gziparchive/)
* сборка [Aspose.Zip](../../../)

---

## GzipArchive(string, bool) {#constructor_2}

Инициализирует новый экземпляр[`GzipArchive`](../) класс.

```csharp
public GzipArchive(string path, bool parseHeader = false)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу архива. |
| parseHeader | Boolean | Следует ли анализировать заголовок потока, чтобы выяснить свойства, включая имя. Имеет смысл только для потока с возможностью поиска. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* нулевой. |
| SecurityException | У вызывающего абонента нет необходимого разрешения на доступ. |
| ArgumentException | *path* пуст, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу*path* отказано. |
| PathTooLongException | Указанный*path*, имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. |
| NotSupportedException | Файл в*path* содержит двоеточие (:) в середине строки. |

### Примечания

Этот конструктор не распаковывается. Видеть[`Open`](../open/) метод распаковки.

### Примеры

Откройте архив из файла по пути и извлеките его в`ПамятьПоток`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive("archive.gz"))
  archive.Open().CopyTo(ms);
```

### Смотрите также

* class [GzipArchive](../)
* пространство имен [Aspose.Zip.Gzip](../../gziparchive/)
* сборка [Aspose.Zip](../../../)


