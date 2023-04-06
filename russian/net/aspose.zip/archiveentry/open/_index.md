---
title: ArchiveEntry.Open
second_title: Aspose.ZIP для справочника API .NET
description: ArchiveEntry метод. Открывает запись для извлечения и предоставляет поток с распакованным содержимым записи.
type: docs
weight: 110
url: /ru/net/aspose.zip/archiveentry/open/
---
## ArchiveEntry.Open method

Открывает запись для извлечения и предоставляет поток с распакованным содержимым записи.

```csharp
public Stream Open(string password = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| password | String | Необязательный пароль для расшифровки. |

### Возвращаемое значение

Поток, представляющий содержимое записи.

### Примечания

Прочитайте из потока, чтобы получить исходное содержимое файла. См. раздел примеров.

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

* class [ArchiveEntry](../)
* пространство имен [Aspose.Zip](../../archiveentry/)
* сборка [Aspose.Zip](../../../)


