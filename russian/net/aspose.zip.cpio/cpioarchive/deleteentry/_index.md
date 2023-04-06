---
title: CpioArchive.DeleteEntry
second_title: Aspose.ZIP для справочника API .NET
description: CpioArchive метод. Удаляет первое вхождение определенной записи из списка записей.
type: docs
weight: 50
url: /ru/net/aspose.zip.cpio/cpioarchive/deleteentry/
---
## DeleteEntry(CpioEntry) {#deleteentry}

Удаляет первое вхождение определенной записи из списка записей.

```csharp
public CpioArchive DeleteEntry(CpioEntry entry)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| entry | CpioEntry | Запись, которую необходимо удалить из списка записей. |

### Возвращаемое значение

Экземпляр записи Cpio.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *entry* нулевой. |

### Примеры

Вот как вы можете удалить все записи, кроме последней:

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputCpioFile);
}
```

### Смотрите также

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* пространство имен [Aspose.Zip.Cpio](../../cpioarchive/)
* сборка [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Удаляет запись из списка записей по индексу.

```csharp
public CpioArchive DeleteEntry(int entryIndex)
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
using (var archive = new CpioArchive("two_files.cpio"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.cpio");
}
```

### Смотрите также

* class [CpioArchive](../)
* пространство имен [Aspose.Zip.Cpio](../../cpioarchive/)
* сборка [Aspose.Zip](../../../)


