---
title: "UueArchive.UueArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор UueArchive. Инициализирует новый экземпляр класса UueArchive, подготовленный для кодирования"
type: docs
weight: 10
url: /ru/net/aspose.zip.uue/uuearchive/uuearchive/
---
## UueArchive() {#constructor}

Инициализирует новый экземпляр класса [`UueArchive`](../), подготовленного для кодирования.

```csharp
public UueArchive()
```

## Примеры

Следующий пример показывает, как выполнить uuencode файла.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.uue");
}
```

### См. также

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(Stream) {#constructor_1}

Инициализирует новый экземпляр класса [`UueArchive`](../), подготовленного для декодирования.

```csharp
public UueArchive(Stream sourceStream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. |

## Примечания

Этот конструктор не декодирует. См. метод [`Open`](../open/) для распаковки.

## Примеры

Откройте архив из потока и извлеките его в `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive(File.OpenRead("archive.001")))
  archive.Open().CopyTo(ms);
```

### См. также

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(string) {#constructor_2}

Инициализирует новый экземпляр класса [`UueArchive`](../).

```csharp
public UueArchive(string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу архива. |

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
| FileNotFoundException | Файл не найден. |
| IOException | Файл уже открыт. |

## Примечания

Этот конструктор не выполняет распаковку. См. метод [`Open`](../open/) для распаковки.

## Примеры

Откройте архив из файла по пути и декодируйте его в `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive("archive.uue"))
  archive.Open().CopyTo(ms);
```

### См. также

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


