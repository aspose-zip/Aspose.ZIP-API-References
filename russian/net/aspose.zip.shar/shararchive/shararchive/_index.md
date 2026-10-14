---
title: "SharArchive.SharArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор SharArchive. Инициализирует новый экземпляр класса SharArchive"
type: docs
weight: 10
url: /ru/net/aspose.zip.shar/shararchive/shararchive/
---
## SharArchive() {#constructor}

Инициализирует новый экземпляр класса [`SharArchive`](../).

```csharp
public SharArchive()
```

## Примеры

В следующем примере показано, как сжать файл.

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### См. также

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## SharArchive(string) {#constructor_1}

Инициализирует новый экземпляр класса [`SharArchive`](../), подготовленный для распаковки.

```csharp
public SharArchive(string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к источнику архива. |

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

### См. также

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


