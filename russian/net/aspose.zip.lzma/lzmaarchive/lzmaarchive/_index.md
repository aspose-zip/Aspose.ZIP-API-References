---
title: "LzmaArchive.LzmaArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор LzmaArchive. Инициализирует новый экземпляр класса LzmaArchive и создает архив в формате lzma."
type: docs
weight: 10
url: /ru/net/aspose.zip.lzma/lzmaarchive/lzmaarchive/
---
## LzmaArchive(LzmaArchiveSettings) {#constructor}

Инициализирует новый экземпляр класса [`LzmaArchive`](../) и создает архив в формате lzma.

```csharp
public LzmaArchive(LzmaArchiveSettings settings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| настройки | LzmaArchiveSettings | Набор настроек конкретного lzma-архива. |

### См. также

* class [LzmaArchiveSettings](../../lzmaarchivesettings/)
* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzmaArchive(Stream) {#constructor_1}

Инициализирует новый экземпляр класса [`LzmaArchive`](../), подготовленный для распаковки.

```csharp
public LzmaArchive(Stream source)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| source | Stream | Источник архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *source* равен null. |

## Примечания

Этот конструктор не распаковывает. См. метод [`Extract`](../extract/) для распаковки.

### См. также

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzmaArchive(string) {#constructor_2}

Инициализирует новый экземпляр класса [`LzmaArchive`](../), подготовленный для распаковки.

```csharp
public LzmaArchive(string path)
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
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| FileNotFoundException | Файл не найден. |
| IOException | Файл уже открыт. |

## Примечания

Этот конструктор не распаковывает. См. метод [`Extract`](../extract/) для распаковки.

## Примеры

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzmaArchive(sourceLzmaFile))
    {
         archive.Extract(extractedFile);
    }
}
```

### См. также

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)


