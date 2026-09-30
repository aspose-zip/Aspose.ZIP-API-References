---
title: "ArchiveEntry.Open"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод ArchiveEntry. Открывает запись для извлечения и предоставляет поток с распакованным содержимым записи."
type: docs
weight: 120
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

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Архив находится в некорректном состоянии. |
| ObjectDisposedException | Выбрасывается, если архив был освобождён. |

## Примечания

Прочитайте из потока, чтобы получить исходное содержимое файла. См. раздел примеров.

## Примеры

Использование:

```csharp
Stream decompressed = entry.Open();
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

* class [ArchiveEntry](../)
* namespace [Aspose.Zip](../../archiveentry/)
* assembly [Aspose.Zip](../../../)


