---
title: "IsoArchive.CreateDirectory"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод IsoArchive. Добавляет каталог в ISO‑образ"
type: docs
weight: 30
url: /ru/net/aspose.zip.iso/isoarchive/createdirectory/
---
## IsoArchive.CreateDirectory method

Добавляет каталог в ISO‑образ.

```csharp
public IsoEntry CreateDirectory(string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Путь к каталогу в ISO. |

### Возвращаемое значение

Элемент ISO составлен.

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Архив открыт для извлечения. |
| ArgumentNullException | `name` имеет значение null или пустой. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

### См. также

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


