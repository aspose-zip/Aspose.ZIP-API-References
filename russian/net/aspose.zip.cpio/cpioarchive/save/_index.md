---
title: CpioArchive.Save
second_title: Aspose.ZIP для справочника API .NET
description: CpioArchive метод. Сохраняет архив в указанный файл назначения.
type: docs
weight: 80
url: /ru/net/aspose.zip.cpio/cpioarchive/save/
---
## Save(string, CpioFormat) {#save_1}

Сохраняет архив в указанный файл назначения.

```csharp
public void Save(string destinationFileName, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | String | Путь создаваемого архива. Если указанное имя файла указывает на существующий файл, он будет перезаписан. |
| cpioFormat | CpioFormat | Определяет формат заголовка cpio. |

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
using (var archive = new CpioArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.cpio");
}       
```

### Смотрите также

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* пространство имен [Aspose.Zip.Cpio](../../cpioarchive/)
* сборка [Aspose.Zip](../../../)

---

## Save(Stream, CpioFormat) {#save}

Сохраняет архив в указанный поток.

```csharp
public void Save(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| output | Stream | Целевой поток. |
| cpioFormat | CpioFormat | Определяет формат заголовка cpio. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *output* нулевой. |
| ArgumentException | *output* не доступен для записи. - или -*output* это тот же поток, из которого мы извлекаем. - ИЛИ - Невозможно сохранить архив в*cpioFormat* из-за ограничений формата. |

### Примечания

*output*должен быть доступен для записи.

### Примеры

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(cpioFile);
    }
}       
```

### Смотрите также

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* пространство имен [Aspose.Zip.Cpio](../../cpioarchive/)
* сборка [Aspose.Zip](../../../)


