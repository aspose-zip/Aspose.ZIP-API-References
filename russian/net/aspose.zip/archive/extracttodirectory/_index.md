---
title: Archive.ExtractToDirectory
second_title: Aspose.ZIP для справочника API .NET
description: Archive метод. Извлекает все файлы из архива в указанный каталог.
type: docs
weight: 80
url: /ru/net/aspose.zip/archive/extracttodirectory/
---
## Archive.ExtractToDirectory method

Извлекает все файлы из архива в указанный каталог.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationDirectory | String | Путь к каталогу для размещения извлеченных файлов. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *destinationDirectory* нулевой. |
| PathTooLongException | Указанный путь, имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. |
| SecurityException | У вызывающего абонента нет необходимого разрешения для доступа к существующему каталогу. |
| NotSupportedException | Если каталог не существует, путь содержит символ двоеточия (:), который не является частью метки диска ("C:\"). |
| ArgumentException | *destinationDirectory*представляет собой строку нулевой длины, содержащую только пробел или один или несколько недопустимых символов. Вы можете запросить недопустимые символы с помощью метода System.IO.Path.GetInvalidPathChars. -или- путь имеет префикс или содержит только символ двоеточия (:). |
| IOException | Каталог, указанный путем, является файлом. -или- Имя сети неизвестно. |
| InvalidDataException | Введен неверный пароль. |

### Примечания

Если каталог не существует, он будет создан.

### Примеры

```csharp
using (var archive = new Archive("archive.zip")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Смотрите также

* class [Archive](../)
* пространство имен [Aspose.Zip](../../archive/)
* сборка [Aspose.Zip](../../../)


