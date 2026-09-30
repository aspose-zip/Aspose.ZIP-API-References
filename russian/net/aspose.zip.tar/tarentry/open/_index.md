---
title: "TarEntry.Open"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод TarEntry. Открывает элемент для извлечения и предоставляет поток с содержимым элемента"
type: docs
weight: 70
url: /ru/net/aspose.zip.tar/tarentry/open/
---
## TarEntry.Open method

Открывает запись для извлечения и предоставляет поток с содержимым записи.

```csharp
public Stream Open()
```

### Возвращаемое значение

Поток, представляющий содержимое записи.

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |
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

* class [TarEntry](../)
* namespace [Aspose.Zip.Tar](../../tarentry/)
* assembly [Aspose.Zip](../../../)


