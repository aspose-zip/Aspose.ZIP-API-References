---
title: Archive.Save
second_title: Aspose.ZIP для справочника API .NET
description: Archive метод. Сохраняет архив в указанный поток.
type: docs
weight: 90
url: /ru/net/aspose.zip/archive/save/
---
## Save(Stream, ArchiveSaveOptions) {#save}

Сохраняет архив в указанный поток.

```csharp
public void Save(Stream outputStream, ArchiveSaveOptions saveOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| outputStream | Stream | Целевой поток. |
| saveOptions | ArchiveSaveOptions | Варианты сохранения архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *outputStream* не доступен для записи. |

### Примечания

*outputStream*должен быть доступен для записи.

### Примеры

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(zipFile);
    }
}
```

### Смотрите также

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* пространство имен [Aspose.Zip](../../archive/)
* сборка [Aspose.Zip](../../../)

---

## Save(string, ArchiveSaveOptions) {#save_1}

Сохраняет архив в указанный файл назначения.

```csharp
public void Save(string destinationFileName, ArchiveSaveOptions saveOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | String | Путь создаваемого архива. Если указанное имя файла указывает на существующий файл, он будет перезаписан. |
| saveOptions | ArchiveSaveOptions | Варианты сохранения архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *destinationFileName* нулевой. |
| SecurityException | У вызывающего абонента нет необходимого разрешения на доступ. |
| ArgumentException | *destinationFileName* пуст, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу*destinationFileName* отказано. |
| PathTooLongException | Указанный*destinationFileName*, имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows длина пути должна быть менее 248 символов, а длина имени файла — менее 260 символов. |
| NotSupportedException | Файл в*destinationFileName* содержит двоеточие (:) в середине строки. |

### Примечания

Архив можно сохранить по тому же пути, по которому он был загружен из . Однако делать это не рекомендуется, поскольку при таком подходе используется копирование во временный файл.

### Примеры

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### Смотрите также

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* пространство имен [Aspose.Zip](../../archive/)
* сборка [Aspose.Zip](../../../)


