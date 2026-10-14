---
title: "CabArchive.ExtractToDirectory"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод CabArchive. Извлекает все файлы из архива в указанную директорию."
type: docs
weight: 60
url: /ru/net/aspose.zip.cab/cabarchive/extracttodirectory/
---
## CabArchive.ExtractToDirectory method

Извлекает все файлы из архива в указанный каталог.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationDirectory | String | Путь к директории, в которую следует поместить извлечённые файлы. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | путь равен null |
| PathTooLongException | Указанный путь, имя файла или их комбинация превышают системно определённую максимальную длину. |
| SecurityException | Вызвавший процесс не имеет необходимого разрешения для доступа к существующей директории. |
| NotSupportedException | Если каталог не существует, путь содержит символ двоеточия (:) который не является частью метки диска ("C:\"). |
| ArgumentException | path является строкой нулевой длины, содержит только пробелы или содержит один или несколько недопустимых символов. Вы можете получить недопустимые символы, используя метод System.IO.Path.GetInvalidPathChars. -или- path начинается с двоеточия или содержит только символ двоеточия (:). |
| IOException | Указанный в пути объект является файлом, а не директорией. -or- Сетевое имя неизвестно. |
| InvalidDataException | Архив повреждён. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| InvalidOperationException | Архив подготовлен к составлению и не может быть извлечён. |
| OperationCanceledException | В .NET Framework 4.0 и выше: Выбрасывается, когда извлечение отменяется с помощью предоставленного токена отмены. |

## Примечания

Если директория не существует, она будет создана.

## Примеры

```csharp
using (var archive = new CabArchive("archive.cab")) 
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### См. также

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


