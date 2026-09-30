---
title: "SharArchive.DeleteEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод SharArchive. Удаляет первое вхождение конкретной записи из списка записей"
type: docs
weight: 50
url: /ru/net/aspose.zip.shar/shararchive/deleteentry/
---
## DeleteEntry(SharEntry) {#deleteentry}

Удаляет первое вхождение конкретной записи из списка записей.

```csharp
public SharArchive DeleteEntry(SharEntry entry)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| запись | SharEntry | Элемент, который нужно удалить из списка элементов. |

### Возвращаемое значение

Экземпляр элемента Shar.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *entry* равно null. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| InvalidOperationException | Этот архив открыт для извлечения. |

## Примеры

Вот как можно удалить все элементы, кроме последнего:

```csharp
using (var archive = new SharArchive("archive.shar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputSharFile);
}
```

### См. также

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Удаляет запись из списка записей по индексу.

```csharp
public SharArchive DeleteEntry(int entryIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| entryIndex | Int32 | Нулевой индекс элемента, который нужно удалить. |

### Возвращаемое значение

Архив с удалённым элементом.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex* меньше 0.-или- *entryIndex* равно или больше количества `Entries` count. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| InvalidOperationException | Этот архив открыт для извлечения. |

## Примеры

```csharp
using (var archive = new SharArchive("two_files.shar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.shar");
}
```

### См. также

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


