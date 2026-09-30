---
title: "XarArchive.XarArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор XarArchive. Инициализирует новый экземпляр класса XarArchive."
type: docs
weight: 10
url: /ru/net/aspose.zip.xar/xararchive/xararchive/
---
## XarArchive(XarCompressionSettings) {#constructor}

Инициализирует новый экземпляр класса [`XarArchive`](../).

```csharp
public XarArchive(XarCompressionSettings defaultCompressionSettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| defaultCompressionSettings | XarCompressionSettings | Настройки сжатия по умолчанию, применяемые ко всем записям архива. |

## Примеры

В следующем примере показано, как сжать файл.

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.xar");
}
```

### См. также

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## XarArchive(Stream, XarLoadOptions) {#constructor_1}

Инициализирует новый экземпляр класса [`XarArchive`](../) и формирует список записей, которые можно извлечь из архива.

```csharp
public XarArchive(Stream sourceStream, XarLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. Должен поддерживать поиск. |
| loadOptions | XarLoadOptions | Параметры загрузки архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *sourceStream* имеет значение null. |
| ArgumentException | *sourceStream* не поддерживает перемещение. |
| InvalidDataException | *sourceStream* не является действительным xar‑архивом. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`Open`](../../xarfileentry/open/) для распаковки.

## Примеры

В следующем примере показано, как извлечь все записи в каталог.

```csharp
using (var archive = new XarArchive(File.OpenRead("archive.xar")))
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### См. также

* class [XarLoadOptions](../../xarloadoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## XarArchive(string, XarLoadOptions) {#constructor_2}

Инициализирует новый экземпляр класса [`XarArchive`](../) и формирует список записей, которые можно извлечь из архива.

```csharp
public XarArchive(string path, XarLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу архива. |
| loadOptions | XarLoadOptions | Параметры загрузки архива. |

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
| InvalidDataException | Файл по пути *path* не является действительным xar‑архивом. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`Open`](../../xarfileentry/open/) для распаковки.

## Примеры

В следующем примере показано, как извлечь все записи в каталог.

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### См. также

* class [XarLoadOptions](../../xarloadoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


