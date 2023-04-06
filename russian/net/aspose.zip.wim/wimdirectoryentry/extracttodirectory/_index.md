---
title: WimDirectoryEntry.ExtractToDirectory
second_title: Aspose.ZIP для справочника API .NET
description: WimDirectoryEntry метод. Извлекает все файлы из текущего каталога в указанный каталог.
type: docs
weight: 50
url: /ru/net/aspose.zip.wim/wimdirectoryentry/extracttodirectory/
---
## WimDirectoryEntry.ExtractToDirectory method

Извлекает все файлы из текущего каталога в указанный каталог.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationDirectory | String | Путь к каталогу для размещения извлеченных файлов. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | путь нулевой |
| PathTooLongException | Указанный путь, имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. |
| SecurityException | У вызывающего абонента нет необходимого разрешения для доступа к существующему каталогу. |
| NotSupportedException | Если каталог не существует, путь содержит символ двоеточия (:), который не является частью метки диска ("C:\"). |
| ArgumentException | path представляет собой строку нулевой длины, содержащую только пробел или один или несколько недопустимых символов. Вы можете запросить недопустимые символы с помощью метода System.IO.Path.GetInvalidPathChars. -или- путь имеет префикс или содержит только символ двоеточия (:). |
| IOException | Каталог, указанный путем, является файлом. -или- Имя сети неизвестно. |

### Примечания

Если каталог не существует, он будет создан.

### Примеры

```csharp
using (var archive = new WimArchive("archive.wim")) 
{ 
   archive.Images[0].RootDirectory.ExtractToDirectory(@"C:\\extracted");
}
```

### Смотрите также

* class [WimDirectoryEntry](../)
* пространство имен [Aspose.Zip.Wim](../../wimdirectoryentry/)
* сборка [Aspose.Zip](../../../)


