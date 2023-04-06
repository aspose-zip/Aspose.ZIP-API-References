---
title: TarArchive.Save
second_title: Aspose.ZIP для справочника API .NET
description: TarArchive метод. Сохраняет архив в указанный поток.
type: docs
weight: 120
url: /ru/net/aspose.zip.tar/tararchive/save/
---
## Save(Stream, TarFormat?) {#save}

Сохраняет архив в указанный поток.

```csharp
public void Save(Stream output, TarFormat? format = default)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| output | Stream | Целевой поток. |
| format | Nullable`1 | Определяет формат заголовка tar. Нулевое значение будет рассматриваться как USTar, когда это возможно. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *output* не доступен для записи. - или -*output* это тот же поток, из которого мы извлекаем. - ИЛИ - Невозможно сохранить архив в*format* из-за ограничений формата. |

### Примечания

*output*должен быть доступен для записи.

### Примеры

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(tarFile);
    }
}       
```

### Смотрите также

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* пространство имен [Aspose.Zip.Tar](../../tararchive/)
* сборка [Aspose.Zip](../../../)

---

## Save(string, TarFormat?) {#save_1}

Сохраняет архив в указанный файл назначения.

```csharp
public void Save(string destinationFileName, TarFormat? format = default)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | String | Путь создаваемого архива. Если указанное имя файла указывает на существующий файл, он будет перезаписан. |
| format | Nullable`1 | Определяет формат заголовка tar. Нулевое значение будет рассматриваться как USTar, когда это возможно. |

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
using (var archive = new TarArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("myarchive.tar");
}       
```

### Смотрите также

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* пространство имен [Aspose.Zip.Tar](../../tararchive/)
* сборка [Aspose.Zip](../../../)


