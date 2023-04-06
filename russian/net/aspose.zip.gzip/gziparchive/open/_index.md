---
title: GzipArchive.Open
second_title: Aspose.ZIP для справочника API .NET
description: GzipArchive метод. Открывает архив для извлечения и предоставляет поток с содержимым архива.
type: docs
weight: 50
url: /ru/net/aspose.zip.gzip/gziparchive/open/
---
## GzipArchive.Open method

Открывает архив для извлечения и предоставляет поток с содержимым архива.

```csharp
public Stream Open()
```

### Возвращаемое значение

Поток, представляющий содержимое архива.

### Примечания

Прочитать из потока, чтобы получить исходное содержимое файла. См. раздел примеров.

### Примеры

Извлекает архив и копирует извлеченное содержимое в файловый поток.

Вы можете использовать метод Stream.CopyTo для .NET 4.0 и выше:

```csharp
unpacked.CopyTo(extracted);
```

```csharp
using (var archive = new GzipArchive("archive.gz"))
{
    using (var extracted = File.Create("data.bin"))
    {
        var unpacked = archive.Open();
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = unpacked.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }            
}
```

### Смотрите также

* class [GzipArchive](../)
* пространство имен [Aspose.Zip.Gzip](../../gziparchive/)
* сборка [Aspose.Zip](../../../)


