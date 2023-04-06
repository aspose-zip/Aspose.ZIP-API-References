---
title: GzipArchive.Extract
second_title: Aspose.ZIP для справочника API .NET
description: GzipArchive метод. Извлекает архив в указанный поток.
type: docs
weight: 40
url: /ru/net/aspose.zip.gzip/gziparchive/extract/
---
## GzipArchive.Extract method

Извлекает архив в указанный поток.

```csharp
public void Extract(Stream destination)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destination | Stream | Целевой поток. Должен быть доступен для записи. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *destination* не поддерживает запись. |

### Примеры

```csharp
using (var archive = new GzipArchive("archive.gz"))
{
     archive.Extract(httpResponseStream);
}
```

### Смотрите также

* class [GzipArchive](../)
* пространство имен [Aspose.Zip.Gzip](../../gziparchive/)
* сборка [Aspose.Zip](../../../)


