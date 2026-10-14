---
title: "XarDirectoryEntry.ExtractToDirectory"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод XarDirectoryEntry. Извлекает все файлы из текущего каталога в указанный каталог"
type: docs
weight: 50
url: /ru/net/aspose.zip.xar/xardirectoryentry/extracttodirectory/
---
## XarDirectoryEntry.ExtractToDirectory method

Извлекает все файлы из текущего каталога в указанный каталог.

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
| PathTooLongException | Указанный путь, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| SecurityException | Вызвавший процесс не имеет необходимого разрешения для доступа к существующей директории. |
| NotSupportedException | Если директория не существует, путь содержит символ двоеточия (:), который не является частью метки диска (\"C:\\"). |
| ArgumentException | path является строкой нулевой длины, содержит только пробелы или содержит один или несколько недопустимых символов. Вы можете получить недопустимые символы, используя метод System.IO.Path.GetInvalidPathChars. -или- path начинается с двоеточия или содержит только символ двоеточия (:). |
| IOException | Указанный в пути объект является файлом, а не директорией. -or- Сетевое имя неизвестно. |
| InvalidDataException | Архив повреждён. |
| OperationCanceledException | В .NET Framework 4.0 и выше: Выбрасывается, когда извлечение отменяется с помощью предоставленного токена отмены. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |

## Примечания

Если директория не существует, она будет создана.

## Примеры

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   ((XarDirectoryEntry)archive.Entries[0]).ExtractToDirectory("C:\\extracted");
}
```

### См. также

* class [XarDirectoryEntry](../)
* namespace [Aspose.Zip.Xar](../../xardirectoryentry/)
* assembly [Aspose.Zip](../../../)


