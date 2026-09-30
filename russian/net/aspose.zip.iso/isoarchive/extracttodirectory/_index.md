---
title: "IsoArchive.ExtractToDirectory"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод IsoArchive. Извлекает все элементы в указанный каталог"
type: docs
weight: 60
url: /ru/net/aspose.zip.iso/isoarchive/extracttodirectory/
---
## IsoArchive.ExtractToDirectory method

Извлекает все записи в указанный каталог.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationDirectory | String | Каталог, в который будут извлечены элементы. |

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Выбрасывается, когда архив находится в режиме редактирования. |
| ArgumentNullException | Выбрасывается, когда *destinationDirectory* имеет значение null. |
| OperationCanceledException | В .NET Framework 4.0 и выше: Выбрасывается, когда извлечение отменяется с помощью предоставленного токена отмены. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примеры

В следующем примере показано, как извлечь все элементы в каталог:

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### См. также

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


