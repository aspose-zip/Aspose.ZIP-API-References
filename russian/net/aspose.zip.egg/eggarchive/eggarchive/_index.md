---
title: "EggArchive.EggArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор EggArchive. Инициализирует новый экземпляр класса EggArchive из потока"
type: docs
weight: 10
url: /ru/net/aspose.zip.egg/eggarchive/eggarchive/
---
## EggArchive(Stream, EggArchiveLoadOptions) {#constructor}

Инициализирует новый экземпляр класса [`EggArchive`](../) из потока.

```csharp
public EggArchive(Stream stream, EggArchiveLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Поток архива EGG. Поток должен поддерживать чтение и перемещение. |
| loadOptions | EggArchiveLoadOptions | Параметры для загрузки архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *stream* равно null. |
| ArgumentException | *stream* не поддерживает чтение и перемещение. |

### См. также

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)

---

## EggArchive(string, EggArchiveLoadOptions) {#constructor_1}

Инициализирует новый экземпляр класса [`EggArchive`](../) из пути к файлу.

```csharp
public EggArchive(string path, EggArchiveLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу архива EGG. |
| loadOptions | EggArchiveLoadOptions | Параметры для загрузки архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* имеет значение null. |
| FileNotFoundException | Файл не существует. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | *path* пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *path* запрещён. |
| PathTooLongException | Указанный *path*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл по адресу *path* содержит двоеточие (:) в середине строки. |
| FileNotFoundException | Файл не найден. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| IOException | Файл уже открыт. |

### См. также

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)


