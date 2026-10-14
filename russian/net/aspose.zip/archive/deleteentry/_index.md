---
title: "Archive.DeleteEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод Archive. Удаляет первое вхождение указанного элемента из списка элементов"
type: docs
weight: 70
url: /ru/net/aspose.zip/archive/deleteentry/
---
## DeleteEntry(ArchiveEntry) {#deleteentry}

Удаляет первое вхождение указанной записи из списка записей.

```csharp
public Archive DeleteEntry(ArchiveEntry entry)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| запись | ArchiveEntry | Элемент, который нужно удалить из списка элементов. |

### Возвращаемое значение

Архив с удалённым элементом.

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Архив освобождён. |
| InvalidOperationException | Выбрасывается, когда удаление элемента недопустимо из‑за текущего состояния архива. |

## Примеры

Вот как можно удалить все элементы, кроме последнего:

```csharp
using (var archive = new Archive("archive.zip"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save("last_entry.zip");
}
```

### См. также

* class [ArchiveEntry](../../archiveentry/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Удаляет запись из списка записей по индексу.

```csharp
public Archive DeleteEntry(int entryIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| entryIndex | Int32 | Нулевой индекс элемента, который нужно удалить. |

### Возвращаемое значение

Архив с удалённым элементом.

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Archive освобождён. |
| ArgumentOutOfRangeException | *entryIndex* меньше 0.-или- *entryIndex* равно или больше количества `Entries` count. |
| InvalidOperationException | Выбрасывается, когда удаление элемента недопустимо из‑за текущего состояния архива. |

## Примеры

```csharp
using (var archive = new TarArchive("two_files.zip"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.zip");
}
```

### См. также

* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


