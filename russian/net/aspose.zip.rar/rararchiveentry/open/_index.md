---
title: "RarArchiveEntry.Open"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод RarArchiveEntry. Открывает запись для извлечения и предоставляет поток с распакованным содержимым записи"
type: docs
weight: 100
url: /ru/net/aspose.zip.rar/rararchiveentry/open/
---
## RarArchiveEntry.Open method

Открывает запись для извлечения и предоставляет поток с распакованным содержимым записи.

```csharp
public Stream Open(string password = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| password | String | Необязательный пароль для расшифровки. Его также можно задать в [`DecryptionPassword`](../../rararchiveloadoptions/decryptionpassword/). |

### Возвращаемое значение

Поток, представляющий содержимое записи.

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

* class [RarArchiveEntry](../)
* namespace [Aspose.Zip.Rar](../../rararchiveentry/)
* assembly [Aspose.Zip](../../../)


