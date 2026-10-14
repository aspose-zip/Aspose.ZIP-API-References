---
title: "GzipArchive.UncompressedSize"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Свойство GzipArchive. Получает размер оригинального файла"
type: docs
weight: 30
url: /ru/net/aspose.zip.gzip/gziparchive/uncompressedsize/
---
## GzipArchive.UncompressedSize property

Получает размер оригинального файла.

```csharp
public ulong UncompressedSize { get; }
```

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примечания

Во время распаковки это свойство может содержать некорректный размер. Если размер распакованного файла превышает 4 ГБ, это свойство будет возвращать неверное значение из‑за 32‑битного ограничения в заголовке.

### См. также

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


