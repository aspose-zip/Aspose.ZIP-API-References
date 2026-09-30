---
title: "Bzip2Archive.Save"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод Bzip2Archive. Сохраняет архив в предоставленный поток."
type: docs
weight: 60
url: /ru/net/aspose.zip.bzip2/bzip2archive/save/
---
## Save(Stream, Bzip2SaveOptions) {#save}

Сохраняет архив в предоставленный поток.

```csharp
public void Save(Stream outputStream, Bzip2SaveOptions saveOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| outputStream | Stream | Поток назначения. |
| saveOptions | Bzip2SaveOptions | Параметры сохранения bzip2‑архива. Если не указано, будет использован размер блока 900 КБ. |

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Источник данных для архивирования не был предоставлен. |
| ArgumentException | *outputStream* недоступен для записи. |
| UnauthorizedAccessException | Источник файла доступен только для чтения или является каталогом. |
| DirectoryNotFoundException | Указанный путь к источнику файла недействителен, например, находится на несвязанном диске. |
| IOException | Источник файла уже открыт. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примечания

*outputStream* must be writable.

## Примеры

Записать сжатые данные в поток ответа http.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### См. также

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, Bzip2SaveOptions) {#save_1}

Сохраняет архив в указанный файл назначения.

```csharp
public void Save(string destinationFileName, Bzip2SaveOptions saveOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | String | Путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан. |
| saveOptions | Bzip2SaveOptions | Параметры сохранения bzip2‑архива. Если не указано, будет использован размер блока 900 КБ. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *destinationFileName* равно null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | *destinationFileName* пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *destinationFileName* запрещён. |
| PathTooLongException | Указанный *destinationFileName*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл в *destinationFileName* содержит двоеточие (:) в середине строки. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| InvalidOperationException | Источник данных для архивирования не был предоставлен. |

## Примеры

Записывает сжатые данные в файл.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bz2");
}
```

### См. также

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)


