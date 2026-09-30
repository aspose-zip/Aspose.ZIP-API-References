---
title: "UueArchive.Save"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод UueArchive. Сохраняет архив в предоставленный поток"
type: docs
weight: 70
url: /ru/net/aspose.zip.uue/uuearchive/save/
---
## Save(Stream, UueSaveOptions) {#save}

Сохраняет архив в предоставленный поток.

```csharp
public void Save(Stream outputStream, UueSaveOptions saveOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| outputStream | Stream | Поток назначения. |
| saveOptions | UueSaveOptions | Параметры сохранения архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| InvalidOperationException | Источник данных для архивирования не был предоставлен. |
| ArgumentException | *outputStream* недоступен для записи. |
| UnauthorizedAccessException | Источник файла доступен только для чтения или является каталогом. |
| DirectoryNotFoundException | Указанный путь к источнику файла недействителен, например, находится на несвязанном диске. |
| IOException | Источник файла уже открыт. |

## Примечания

*outputStream* must be writable.

## Примеры

Записать сжатые данные в поток ответа http.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### См. также

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, UueSaveOptions) {#save_1}

Сохраняет архив в указанный файл назначения.

```csharp
public void Save(string destinationFileName, UueSaveOptions saveOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | String | Путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан. |
| saveOptions | UueSaveOptions | Параметры сохранения архива. |

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
| InvalidOperationException | Источник данных для архивирования не был предоставлен. |

## Примеры

Записать закодированные данные в файл.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.uue");
}
```

### См. также

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


