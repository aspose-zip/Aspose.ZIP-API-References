---
title: "CabArchive.Save"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод CabArchive. Сохраняет архив в предоставленный поток."
type: docs
weight: 70
url: /ru/net/aspose.zip.cab/cabarchive/save/
---
## Save(Stream, CabSaveOptions) {#save}

Сохраняет архив в предоставленный поток.

```csharp
public void Save(Stream outputStream, CabSaveOptions saveOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| outputStream | Stream | Поток назначения. |
| saveOptions | CabSaveOptions | Параметры сохранения архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *outputStream* не поддерживает запись и перемещение. |
| ObjectDisposedException | Архив освобождён. |
| InvalidOperationException | Архив подготовлен к извлечению и не может быть сохранён. |

## Примечания

*outputStream* must be writable.

## Примеры

```csharp
using (FileStream cabFile = File.Open("archive.cab", FileMode.Create))
{
    using (var archive = new CabArchive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(cabFile);
    }
}
```

### См. также

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, CabSaveOptions) {#save_1}

Сохраняет архив в указанный файл назначения.

```csharp
public void Save(string destinationFileName, CabSaveOptions saveOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | String | Путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан. |
| saveOptions | CabSaveOptions | Параметры сохранения архива. |

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
| InvalidOperationException | Архив открыт для извлечения. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| IOException | Файл уже открыт. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

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

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


