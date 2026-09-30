---
title: "XzArchive.XzArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор XzArchive. Инициализирует новый экземпляр класса XzArchive и создает архив в формате xz"
type: docs
weight: 10
url: /ru/net/aspose.zip.xz/xzarchive/xzarchive/
---
## XzArchive(XzArchiveSettings) {#constructor}

Инициализирует новый экземпляр класса [`XzArchive`](../) и создает архив в формате xz.

```csharp
public XzArchive(XzArchiveSettings settings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| настройки | XzArchiveSettings | Набор параметров конкретного xz‑архива: размер словаря, размер блока, тип проверки. |

### См. также

* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [XzArchive](../)
* namespace [Aspose.Zip.Xz](../../xzarchive/)
* assembly [Aspose.Zip](../../../)

---

## XzArchive(Stream, XzLoadOptions) {#constructor_1}

Инициализирует новый экземпляр класса [`XzArchive`](../), подготовленный для распаковки.

```csharp
public XzArchive(Stream source, XzLoadOptions options = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| source | Stream | Источник архива. |
| параметры | XzLoadOptions | Параметры для загрузки архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *source* не поддерживает поиск. |
| ArgumentNullException | *source* равен null. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |
| IOException | Произошла ошибка ввода/вывода. |
| InvalidDataException | Данные недействительны или повреждены. |

## Примечания

Этот конструктор не распаковывает. См. метод [`Extract`](../extract/) для распаковки.

### См. также

* class [XzLoadOptions](../../../aspose.zip.xz.settings/xzloadoptions/)
* class [XzArchive](../)
* namespace [Aspose.Zip.Xz](../../xzarchive/)
* assembly [Aspose.Zip](../../../)

---

## XzArchive(string, XzLoadOptions) {#constructor_2}

Инициализирует новый экземпляр класса [`XzArchive`](../), подготовленный для распаковки.

```csharp
public XzArchive(string path, XzLoadOptions options = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к источнику архива. |
| параметры | XzLoadOptions | Параметры для загрузки архива. |

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
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| InvalidDataException | Выбрасывается, когда данные недействительны или повреждены. |

## Примечания

Этот конструктор не распаковывает. См. метод [`Extract`](../extract/) для распаковки.

### См. также

* class [XzLoadOptions](../../../aspose.zip.xz.settings/xzloadoptions/)
* class [XzArchive](../)
* namespace [Aspose.Zip.Xz](../../xzarchive/)
* assembly [Aspose.Zip](../../../)


