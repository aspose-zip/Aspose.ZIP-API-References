---
title: "CabArchive.CreateEntries"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод CabArchive. Добавляет в архив все файлы рекурсивно из указанного каталога."
type: docs
weight: 30
url: /ru/net/aspose.zip.cab/cabarchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Добавляет в архив все файлы, рекурсивно, из указанного каталога.

```csharp
public CabArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| directory | DirectoryInfo | Каталог для сжатия. |
| includeRootDirectory | Boolean | Указывает, следует ли включать имя корневого каталога в пути записей. |

### Возвращаемое значение

Текущий экземпляр [`CabArchive`](../).

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *directory* равно null. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| DirectoryNotFoundException | *directory* не найден. |
| SecurityException | Вызвавший процесс не имеет необходимого разрешения для доступа к *directory* или его содержимому. |
| UnauthorizedAccessException | Доступ к *directory* или одному из его файлов запрещён. |
| IOException | Произошла ошибка ввода/вывода при доступе к *directory*. |
| PathTooLongException | Сгенерированный путь записи превышает системно определённую максимальную длину. |
| InvalidOperationException | Архив подготовлен к извлечению и не может добавлять записи. |

## Примеры

```csharp
using (var archive = new CabArchive())
{
    var directory = new DirectoryInfo("logs");
    archive.CreateEntries(directory);
    archive.Save("logs.cab");
}
```

### См. также

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Добавляет в архив все файлы рекурсивно из указанного пути к каталогу.

```csharp
public CabArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceDirectory | String | Путь к каталогу для сжатия. |
| includeRootDirectory | Boolean | Указывает, следует ли включать имя корневого каталога в пути записей. |

### Возвращаемое значение

Текущий экземпляр [`CabArchive`](../).

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| ArgumentNullException | *sourceDirectory* имеет значение null. |
| DirectoryNotFoundException | *sourceDirectory* не найден. |
| SecurityException | У вызывающего нет необходимого разрешения для доступа к *sourceDirectory*. |
| UnauthorizedAccessException | Доступ к *sourceDirectory* запрещён. |
| PathTooLongException | Указанный *sourceDirectory* превышает системно определённую максимальную длину. |
| ArgumentException | *sourceDirectory* пуст, содержит только пробелы или содержит недопустимые символы. |
| IOException | Произошла ошибка ввода/вывода при доступе к *sourceDirectory*. |
| InvalidOperationException | Архив подготовлен к извлечению и не может добавлять записи. |

## Примеры

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabStoreCompressionSettings())))
{
    archive.CreateEntries("data", includeRootDirectory: false);
    archive.Save("stored_data.cab");
}
```

### См. также

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


