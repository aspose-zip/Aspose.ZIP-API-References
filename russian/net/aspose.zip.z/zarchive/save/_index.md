---
title: "ZArchive.Save"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод ZArchive. Сохраняет xz‑архив в указанный поток"
type: docs
weight: 50
url: /ru/net/aspose.zip.z/zarchive/save/
---
## Save(Stream, ZArchiveSaveOptions) {#save}

Сохраняет архив xz в указанный поток.

```csharp
public void Save(Stream output, ZArchiveSaveOptions settings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| output | Stream | Поток назначения. |
| настройки | ZArchiveSaveOptions | Необязательные параметры для составления архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| ArgumentException | *output* не поддерживает перемотку. |
| ArgumentNullException | *output* равен null. |

## Примечания

*output* must be seekable.

## Примеры

```csharp
using (FileStream zFile = File.Open("data.bin.z", FileMode.Create))
{
    using (var archive = new ZArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(zFile);
     }
}
```

### См. также

* class [ZArchiveSaveOptions](../../zarchivesaveoptions/)
* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, ZArchiveSaveOptions) {#save_1}

Сохраняет архив Z в указанный файл назначения.

```csharp
public void Save(string destinationFileName, ZArchiveSaveOptions settings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | String | +Путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан. |
| настройки | ZArchiveSaveOptions | Необязательные параметры для составления архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| ArgumentNullException | *destinationFileName* равно null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | *destinationFileName* пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *destinationFileName* запрещён. |
| PathTooLongException | Указанный *destinationFileName*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл в *destinationFileName* содержит двоеточие (:) в середине строки. |
| IOException | Во время открытия файла произошла ошибка ввода/вывода. |

## Примеры

```csharp
using (var archive = new ZArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bin.Z");
}
```

### См. также

* class [ZArchiveSaveOptions](../../zarchivesaveoptions/)
* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)


