---
title: SharArchive.DeleteEntry
second_title: Aspose.ZIP для справочника API .NET
description: SharArchive метод. Удаляет первое вхождение определенной записи из списка записей.
type: docs
weight: 50
url: /ru/net/aspose.zip.shar/shararchive/deleteentry/
---
## DeleteEntry(SharEntry) {#deleteentry}

Удаляет первое вхождение определенной записи из списка записей.

```csharp
public SharArchive DeleteEntry(SharEntry entry)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| entry | SharEntry | Запись, которую необходимо удалить из списка записей. |

### Возвращаемое значение

Экземпляр записи Shar.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *entry* нулевой. |

### Примеры

Вот как вы можете удалить все записи, кроме последней:

```csharp
using (var archive = new SharArchive("archive.shar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputSharFile);
}
```

### Смотрите также

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* пространство имен [Aspose.Zip.Shar](../../shararchive/)
* сборка [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Удаляет запись из списка записей по индексу.

```csharp
public SharArchive DeleteEntry(int entryIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| entryIndex | Int32 | Отсчитываемый от нуля индекс удаляемой записи. |

### Возвращаемое значение

Архив с записью удален.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex* меньше 0.-или-*entryIndex* равно или больше, чем`Записи` считать. |

### Примеры

```csharp
using (var archive = new SharArchive("two_files.shar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.shar");
}
```

### Смотрите также

* class [SharArchive](../)
* пространство имен [Aspose.Zip.Shar](../../shararchive/)
* сборка [Aspose.Zip](../../../)


