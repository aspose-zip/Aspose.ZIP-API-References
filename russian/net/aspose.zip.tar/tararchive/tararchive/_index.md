---
title: "TarArchive.TarArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор TarArchive. Инициализирует новый экземпляр класса TarArchive"
type: docs
weight: 10
url: /ru/net/aspose.zip.tar/tararchive/tararchive/
---
## TarArchive() {#constructor}

Инициализирует новый экземпляр класса [`TarArchive`](../).

```csharp
public TarArchive()
```

## Примеры

В следующем примере показано, как сжать файл.

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.tar");
}
```

### См. также

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## TarArchive(Stream, TarLoadOptions) {#constructor_1}

Инициализирует новый экземпляр класса [`TarArchive`](../) и формирует список записей, которые можно извлечь из архива.

```csharp
public TarArchive(Stream sourceStream, TarLoadOptions loadOptions = null)
```

| Параметр | Описание |
| --- | --- |
| sourceStream | Источник архива. Должен поддерживать поиск. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *sourceStream* не поддерживает перемещение. |
| ArgumentNullException | *sourceStream* имеет значение null. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`Open`](../../tarentry/open/) для распаковки.

## Примеры

В следующем примере показано, как извлечь все записи в каталог.

```csharp
using (var archive = new TarArchive(File.OpenRead("archive.tar")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### См. также

* class [TarLoadOptions](../../tarloadoptions/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## TarArchive(string, TarLoadOptions) {#constructor_2}

Инициализирует новый экземпляр класса [`TarArchive`](../) и формирует список записей, которые можно извлечь из архива.

```csharp
public TarArchive(string path, TarLoadOptions loadOptions = null)
```

| Параметр | Описание |
| --- | --- |
| path | Путь к файлу архива. |

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

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`Open`](../../tarentry/open/) для распаковки.

## Примеры

В следующем примере показано, как извлечь все записи в каталог.

```csharp
using (var archive = new TarArchive("archive.tar", new TarLoadOptions() { CancellationToken = cancellationToken }))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### См. также

* class [TarLoadOptions](../../tarloadoptions/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


