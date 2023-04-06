---
title: WimFileEntry.Open
second_title: Aspose.ZIP для справочника API .NET
description: WimFileEntry метод. Открывает запись для извлечения и предоставляет поток с содержимым записи.
type: docs
weight: 30
url: /ru/net/aspose.zip.wim/wimfileentry/open/
---
## WimFileEntry.Open method

Открывает запись для извлечения и предоставляет поток с содержимым записи.

```csharp
public Stream Open()
```

### Возвращаемое значение

Поток, представляющий содержимое записи.

### Примечания

Прочитать из потока, чтобы получить исходное содержимое файла. См. раздел примеров.

### Примеры

Использование:

.NET 4.0 и выше — используйте метод Stream.CopyTo:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 и более ранние версии — копировать байты вручную:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

```csharp
Stream decompressed = entry.Open();
```

### Смотрите также

* class [WimFileEntry](../)
* пространство имен [Aspose.Zip.Wim](../../wimfileentry/)
* сборка [Aspose.Zip](../../../)


