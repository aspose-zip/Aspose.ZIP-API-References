---
title: "ZstandardArchive.Save"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод ZstandardArchive. Сохраняет архив в предоставленный поток"
type: docs
weight: 60
url: /ru/net/aspose.zip.zstandard/zstandardarchive/save/
---
## Save(Stream, ZstandardSaveOptions) {#save_1}

Сохраняет архив в предоставленный поток.

```csharp
public void Save(Stream outputStream, ZstandardSaveOptions settings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| outputStream | Stream | Поток назначения. |
| настройки | ZstandardSaveOptions | Необязательные параметры для составления архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| ArgumentException | *outputStream* недоступен для записи. |
| InvalidOperationException | Источник не был предоставлен. |

## Примечания

*outputStream* must be writable.

## Примеры

Записать сжатые данные в поток ответа http.

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### См. также

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, ZstandardSaveOptions) {#save_2}

Сохраняет архив в указанный файл назначения.

```csharp
public void Save(string destinationFileName, ZstandardSaveOptions settings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | String | Путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан. |
| настройки | ZstandardSaveOptions | Необязательные параметры для составления архива. |

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
| Exception | Выбрасывается, когда происходит ошибка выполнения. |
| DirectoryNotFoundException | Указанный путь недействителен (например, он находится на не смонтированном диске). |
| IOException | Во время открытия файла произошла ошибка ввода/вывода. |
| InvalidOperationException | Источник не был предоставлен. |

## Примеры

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.zst");
}
```

### См. также

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo, ZstandardSaveOptions) {#save}

Сохраняет архив в указанный файл назначения.

```csharp
public void Save(FileInfo destination, ZstandardSaveOptions settings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | FileInfo | FileInfo, который будет открыт как поток назначения. |
| настройки | ZstandardSaveOptions | Необязательные параметры для составления архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| SecurityException | Вызвавший код не имеет необходимого разрешения для открытия *destination*. |
| ArgumentException | Путь к файлу пустой или содержит только пробелы. |
| FileNotFoundException | Файл не найден. |
| UnauthorizedAccessException | Путь к файлу доступен только для чтения или является каталогом. |
| ArgumentNullException | *destination* равно null. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| IOException | Файл уже открыт. |
| InvalidOperationException | Источник не был предоставлен. |

## Примеры

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.zst"));
}
```

### См. также

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


