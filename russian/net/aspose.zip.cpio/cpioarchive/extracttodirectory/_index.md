---
title: "CpioArchive.ExtractToDirectory"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод CpioArchive. Извлекает все файлы из архива в указанный каталог."
type: docs
weight: 70
url: /ru/net/aspose.zip.cpio/cpioarchive/extracttodirectory/
---
## CpioArchive.ExtractToDirectory method

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
| ArgumentNullException | Path имеет значение null |
| PathTooLongException | Указанный путь, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| SecurityException | Вызвавший процесс не имеет необходимого разрешения для доступа к существующей директории. |
| NotSupportedException | Если каталог не существует, путь содержит символ двоеточия (:) который не является частью метки диска ("C:\"). |
| ArgumentException | Path является строкой нулевой длины, содержит только пробелы или содержит один или несколько недопустимых символов. Вы можете получить недопустимые символы, используя метод System.IO.Path.GetInvalidPathChars. -или- путь начинается с двоеточия или содержит только двоеточие (:). |
| IOException | Указанный в пути объект является файлом, а не директорией. -or- Сетевое имя неизвестно. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примечания

Если директория не существует, она будет создана.

## Примеры

```csharp
using (var archive = new CpioArchive("archive.cpio")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### См. также

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


