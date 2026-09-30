---
title: "CpioArchive.DeleteEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод CpioArchive. Удаляет первое вхождение конкретной записи из списка записей."
type: docs
weight: 50
url: /ru/net/aspose.zip.cpio/cpioarchive/deleteentry/
---
## DeleteEntry(CpioEntry) {#deleteentry}

Удаляет первое вхождение конкретной записи из списка записей.

```csharp
public CpioArchive DeleteEntry(CpioEntry entry)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| запись | CpioEntry | Элемент, который нужно удалить из списка элементов. |

### Возвращаемое значение

Экземпляр записи Cpio.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *entry* равно null. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примеры

Вот как можно удалить все элементы, кроме последнего:

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputCpioFile);
}
```

### См. также

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Удаляет запись из списка записей по индексу.

```csharp
public CpioArchive DeleteEntry(int entryIndex)
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

## Примеры

```csharp
using (var archive = new CpioArchive("two_files.cpio"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.cpio");
}
```

### См. также

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


