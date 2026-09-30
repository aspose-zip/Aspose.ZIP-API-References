---
title: "GzipArchive.Open"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод GzipArchive. Открывает архив для извлечения и предоставляет поток с содержимым архива"
type: docs
weight: 70
url: /ru/net/aspose.zip.gzip/gziparchive/open/
---
## GzipArchive.Open method

Открывает архив для извлечения и предоставляет поток с содержимым архива.

```csharp
public Stream Open()
```

### Возвращаемое значение

Поток, представляющий содержимое архива.

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примечания

Прочитайте из потока, чтобы получить исходное содержимое файла. См. раздел примеров.

## Примеры

Извлекает архив и копирует извлечённое содержимое в файловый поток.

```csharp
using (var archive = new GzipArchive("archive.gz"))
{
    using (var extracted = File.Create("data.bin"))
    {
        using(var unpacked = archive.Open())
        {
            byte[] b = new byte[8192];
            int bytesRead;
            while (0 < (bytesRead = unpacked.Read(b, 0, b.Length)))
                extracted.Write(b, 0, bytesRead);
        }
    }            
}
```

Вы можете использовать метод Stream.CopyTo для .NET 4.0 и выше:

```csharp
unpacked.CopyTo(extracted);
```

### См. также

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


