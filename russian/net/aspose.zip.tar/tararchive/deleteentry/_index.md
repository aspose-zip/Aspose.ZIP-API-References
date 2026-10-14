---
title: "TarArchive.DeleteEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод TarArchive. Удаляет первое вхождение конкретного элемента из списка записей"
type: docs
weight: 120
url: /ru/net/aspose.zip.tar/tararchive/deleteentry/
---
## DeleteEntry(TarEntry) {#deleteentry}

Удаляет первое вхождение конкретной записи из списка записей.

```csharp
public TarArchive DeleteEntry(TarEntry entry)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| запись | TarEntry | Элемент, который нужно удалить из списка элементов. |

### Возвращаемое значение

Архив с удалённым элементом.

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Архив был освобождён и не может быть использован |

## Примеры

Вот как можно удалить все элементы, кроме последнего:

```csharp
using (var archive = new TarArchive("archive.tar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputTarFile);
}
```

### См. также

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Удаляет запись из списка записей по индексу.

```csharp
public TarArchive DeleteEntry(int entryIndex)
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
| ObjectDisposedException | Архив был освобождён и не может быть использован |

## Примеры

```csharp
using (var archive = new TarArchive("two_files.tar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.tar");
}
```

### См. также

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


