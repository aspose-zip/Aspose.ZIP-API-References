---
title: "Archive.ExtractToDirectory"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод Archive. Извлекает все файлы из архива в указанную директорию."
type: docs
weight: 90
url: /ru/net/aspose.zip/archive/extracttodirectory/
---
## Archive.ExtractToDirectory method

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
| ArgumentNullException | *destinationDirectory* равно null. |
| PathTooLongException | Указанный путь, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| SecurityException | Вызвавший процесс не имеет необходимого разрешения для доступа к существующей директории. |
| NotSupportedException | Если директория не существует, путь содержит символ двоеточия (:), который не является частью метки диска (\"C:\\"). |
| ArgumentException | *destinationDirectory* является строкой нулевой длины, содержит только пробелы или содержит один или несколько недопустимых символов. Вы можете получить список недопустимых символов, используя метод System.IO.Path.GetInvalidPathChars. -or- путь начинается с двоеточия (:) или содержит только двоеточие. |
| IOException | Указанный в пути объект является файлом, а не директорией. -or- Сетевое имя неизвестно. |
| InvalidDataException | Указан неверный пароль. - or - Архив повреждён. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| EndOfStreamException | Поток не содержит достаточного количества байтов для чтения запрошенных данных. |

## Примечания

Если директория не существует, она будет создана.

## Примеры

```csharp
using (var archive = new Archive("archive.zip")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### См. также

* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


