---
title: "ArjArchive.ExtractToDirectory"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод ArjArchive. Извлекает все записи в указанный каталог"
type: docs
weight: 60
url: /ru/net/aspose.zip.arj/arjarchive/extracttodirectory/
---
## ArjArchive.ExtractToDirectory method

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
| ArgumentNullException | Выбрасывается, когда *destinationDirectory* имеет значение null. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| OperationCanceledException | В .NET Framework 4.0 и выше: Выбрасывается, когда извлечение отменяется с помощью предоставленного токена отмены. |
| InvalidDataException | Несоответствие контрольной суммы заголовков или данных. - или - Архив повреждён. |
| NotImplementedException | Запись сжата методом 4. |

## Примеры

В следующем примере показано, как извлечь все элементы в каталог:

```csharp
using (var archive = new ArjArchive(File.OpenRead("archive.arj")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### См. также

* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


