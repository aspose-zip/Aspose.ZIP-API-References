---
title: "Archive.Save"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод Archive. Сохраняет архив в предоставленный поток."
type: docs
weight: 100
url: /ru/net/aspose.zip/archive/save/
---
## Save(Stream, ArchiveSaveOptions) {#save}

Сохраняет архив в предоставленный поток.

```csharp
public void Save(Stream outputStream, ArchiveSaveOptions saveOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| outputStream | Stream | Поток назначения. |
| saveOptions | ArchiveSaveOptions | Параметры сохранения архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *outputStream* недоступен для записи. |
| ObjectDisposedException | Архив освобождён. |
| InvalidOperationException | Выбрасывается, когда применяется шифрование к уже зашифрованным записям. |

## Примечания

*outputStream* must be writable.

## Примеры

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

### См. также

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, ArchiveSaveOptions) {#save_1}

Сохраняет архив в указанный файл назначения.

```csharp
public void Save(string destinationFileName, ArchiveSaveOptions saveOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | String | Путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан. |
| saveOptions | ArchiveSaveOptions | Параметры сохранения архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *destinationFileName* равно null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | *destinationFileName* пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *destinationFileName* запрещён. |
| PathTooLongException | Указанный *destinationFileName*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл в *destinationFileName* содержит двоеточие (:) в середине строки. |
| FileNotFoundException | Файл не найден. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| IOException | Файл уже открыт. |
| ObjectDisposedException | Выбрасывается, если архив был освобождён. |
| InvalidOperationException | Выбрасывается, когда применяется шифрование к уже зашифрованным записям. |

## Примечания

Можно сохранить архив в тот же путь, из которого он был загружен. Однако это не рекомендуется, потому что такой подход использует копирование во временный файл.

## Примеры

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### См. также

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


