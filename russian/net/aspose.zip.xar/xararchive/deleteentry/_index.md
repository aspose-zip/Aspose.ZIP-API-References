---
title: "XarArchive.DeleteEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод XarArchive. Удаляет первое вхождение указанной записи из списка записей."
type: docs
weight: 50
url: /ru/net/aspose.zip.xar/xararchive/deleteentry/
---
## XarArchive.DeleteEntry method

Удаляет первое вхождение конкретной записи из списка записей.

```csharp
public XarArchive DeleteEntry(XarEntry entry)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| запись | XarEntry | Элемент, который нужно удалить из списка элементов. |

### Возвращаемое значение

Экземпляр записи Xar.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *entry* равно null. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| InvalidOperationException | Архив не открыт для извлечения. |

## Примеры

Вот как можно удалить все элементы, кроме последнего:

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries.FirstOrDefault());
    archive.Save(outputXarFile);
}
```

### См. также

* class [XarEntry](../../xarentry/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


