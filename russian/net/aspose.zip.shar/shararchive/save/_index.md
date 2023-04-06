---
title: SharArchive.Save
second_title: Aspose.ZIP для справочника API .NET
description: SharArchive метод. Сохраняет архив в указанный файл назначения.
type: docs
weight: 70
url: /ru/net/aspose.zip.shar/shararchive/save/
---
## Save(string) {#save_1}

Сохраняет архив в указанный файл назначения.

```csharp
public void Save(string destinationFileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | String | Путь создаваемого архива. Если указанное имя файла указывает на существующий файл, он будет перезаписан. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *destinationFileName* представляет собой строку нулевой длины, содержащую только пробелы или один или несколько недопустимых символов, как определено в System.IO.Path.InvalidPathChars. |
| ArgumentNullException | *destinationFileName* нулевой. |
| PathTooLongException | Указанный*destinationFileName*, имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. |
| DirectoryNotFoundException | Указанный*destinationFileName* недействителен (например, он находится на несопоставленном диске). |
| IOException | Ошибка ввода-вывода при открытии файла. |
| UnauthorizedAccessException | *destinationFileName* указан файл, доступный только для чтения, и доступ не для чтения.-или- путь указан к каталогу.-или- у вызывающего абонента нет необходимых разрешений. |
| NotSupportedException | *destinationFileName* имеет недопустимый формат. |

### Примечания

Архив можно сохранить по тому же пути, по которому он был загружен из . Однако делать это не рекомендуется, поскольку при таком подходе используется копирование во временный файл.

### Примеры

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.shar");
}       
```

### Смотрите также

* class [SharArchive](../)
* пространство имен [Aspose.Zip.Shar](../../shararchive/)
* сборка [Aspose.Zip](../../../)

---

## Save(Stream) {#save}

Сохраняет архив в указанный поток.

```csharp
public void Save(Stream output)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| output | Stream | Целевой поток. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *output* нулевой. |
| ArgumentException | *output* не доступен для записи. - или -*output* это тот же поток, из которого мы извлекаем. |

### Примечания

*output*должен быть доступен для записи.

### Примеры

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(sharFile);
    }
}       
```

### Смотрите также

* class [SharArchive](../)
* пространство имен [Aspose.Zip.Shar](../../shararchive/)
* сборка [Aspose.Zip](../../../)


