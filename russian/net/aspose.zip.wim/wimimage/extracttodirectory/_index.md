---
title: "WimImage.ExtractToDirectory"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод WimImage. Извлекает все файлы из образа в указанный каталог"
type: docs
weight: 40
url: /ru/net/aspose.zip.wim/wimimage/extracttodirectory/
---
## WimImage.ExtractToDirectory method

Извлекает все файлы из образа в указанный каталог.

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

## Примечания

Если директория не существует, она будет создана.

## Примеры

```csharp
using (var archive = new WimArchive("install.wim")) 
{ 
   archive.Images[0].ExtractToDirectory("C:\\extracted");
}
```

### См. также

* class [WimImage](../)
* namespace [Aspose.Zip.Wim](../../wimimage/)
* assembly [Aspose.Zip](../../../)


