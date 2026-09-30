---
title: "Lz4Archive.Open"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Lz4Archive метод. Открывает архив для извлечения и предоставляет поток с содержимым архива"
type: docs
weight: 50
url: /ru/net/aspose.zip.lz4/lz4archive/open/
---
## Lz4Archive.Open method

Открывает архив для извлечения и предоставляет поток с содержимым архива.

```csharp
public Stream Open()
```

### Возвращаемое значение

Поток, представляющий содержимое архива.

### Исключения

| исключение | условие |
| --- | --- |
| EndOfStreamException | Исходный поток слишком короткий. |
| InvalidDataException | Обнаружены неверные байты при инициализации декодирования. |
| InvalidOperationException | Архив подготовлен для компоновки. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| IOException | Произошла ошибка ввода/вывода. |

## Примечания

Прочитайте из потока, чтобы получить исходное содержимое файла. См. раздел примеров.

## Примеры

Извлекает архив и копирует извлечённое содержимое в файловый поток.

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
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

Вы можете использовать метод Stream.CopyTo для .NET 4.0 и выше:

```csharp
unpacked.CopyTo(extracted);
```

### См. также

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


