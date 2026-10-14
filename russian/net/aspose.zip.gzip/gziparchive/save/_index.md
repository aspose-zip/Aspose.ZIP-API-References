---
title: "GzipArchive.Save"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод GzipArchive. Сохраняет архив в предоставленный поток"
type: docs
weight: 80
url: /ru/net/aspose.zip.gzip/gziparchive/save/
---
## Save(Stream) {#save}

Сохраняет архив в предоставленный поток.

```csharp
public void Save(Stream outputStream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| outputStream | Stream | Поток назначения. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *outputStream* недоступен для записи. |
| InvalidOperationException | Источник не был предоставлен. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примечания

*outputStream* must be writable.

## Примеры

Записывает сжатые данные в поток HTTP‑ответа.

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### См. также

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Сохраняет архив в указанный файл назначения.

```csharp
public void Save(string destinationFileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | String | Путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан. |

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

## Примеры

```csharp
using (var archive = new GzipArchive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### См. также

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


