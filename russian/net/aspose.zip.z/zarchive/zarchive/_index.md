---
title: "ZArchive.ZArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор ZArchive. Инициализирует новый экземпляр класса ZArchive, подготовленный для сжатия"
type: docs
weight: 10
url: /ru/net/aspose.zip.z/zarchive/zarchive/
---
## ZArchive() {#constructor}

Инициализирует новый экземпляр класса [`ZArchive`](../), подготовленного для сжатия.

```csharp
public ZArchive()
```

### См. также

* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZArchive(Stream, ZArchiveLoadOptions) {#constructor_1}

Инициализирует новый экземпляр класса [`ZArchive`](../), подготовленного для распаковки.

```csharp
public ZArchive(Stream source, ZArchiveLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| source | Stream | Источник архива. |
| loadOptions | ZArchiveLoadOptions | Параметры загрузки архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *source* не поддерживает поиск. |
| ArgumentNullException | *source* равен null. |

## Примечания

Этот конструктор не распаковывает. См. метод [`Extract`](../extract/) для распаковки.

### См. также

* class [ZArchiveLoadOptions](../../zarchiveloadoptions/)
* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZArchive(string, ZArchiveLoadOptions) {#constructor_2}

Инициализирует новый экземпляр класса [`ZArchive`](../), подготовленного для распаковки.

```csharp
public ZArchive(string path, ZArchiveLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к источнику архива. |
| loadOptions | ZArchiveLoadOptions | Параметры загрузки архива. |

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

## Примечания

Этот конструктор не распаковывает. См. метод [`Extract`](../extract/) для распаковки.

### См. также

* class [ZArchiveLoadOptions](../../zarchiveloadoptions/)
* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)


