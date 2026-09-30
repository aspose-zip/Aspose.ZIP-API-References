---
title: "UueArchive.Open"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод UueArchive. Открывает архив для декодирования и предоставляет поток с содержимым архива"
type: docs
weight: 60
url: /ru/net/aspose.zip.uue/uuearchive/open/
---
## UueArchive.Open method

Открывает архив для декодирования и предоставляет поток с содержимым архива.

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

Использование:

```csharp
Stream decompressed = archive.Open();
```

.NET 4.0 и выше — используйте метод Stream.CopyTo:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 и ниже — копируйте байты вручную:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

### См. также

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


