---
title: "CabEntry.Open"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод CabEntry. Открывает запись для извлечения и предоставляет поток с содержимым записи"
type: docs
weight: 50
url: /ru/net/aspose.zip.cab/cabentry/open/
---
## CabEntry.Open method

Открывает запись для извлечения и предоставляет поток с содержимым записи.

```csharp
public Stream Open()
```

### Возвращаемое значение

Поток, представляющий содержимое записи.

### Исключения

| исключение | условие |
| --- | --- |
| NotSupportedException | Инициализация потока не удалась из‑за неверных данных. |
| InvalidDataException | Архив повреждён. |
| InvalidOperationException | Запись принадлежит архиву, подготовленному для компоновки. |
| ObjectDisposedException | Выбрасывается, если источник был освобождён. |
| IOException | Произошла ошибка ввода/вывода. |

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

* class [CabEntry](../)
* namespace [Aspose.Zip.Cab](../../cabentry/)
* assembly [Aspose.Zip](../../../)


