---
title: "LzipArchive.Save"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод LzipArchive. Сохраняет lzip-архив в предоставленный поток"
type: docs
weight: 70
url: /ru/net/aspose.zip.lzip/lziparchive/save/
---
## Save(Stream) {#save_1}

Сохраняет lzip-архив в указанный поток.

```csharp
public void Save(Stream outputStream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| outputStream | Stream | Поток назначения. |

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| ArgumentException | *outputStream* не поддерживает перемещение. |
| ArgumentNullException | *outputStream* равен null. |
| IOException | Произошла ошибка ввода/вывода. |

## Примечания

*outputStream* must be seekable.

## Примеры

```csharp
using (FileStream lzFile = File.Open("archive.lz", FileMode.Create))
{
    using (var archive = new LzipArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(lzFile);
     }
}
```

### См. также

* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

Сохраняет lzip-архив в указанный файл назначения.

```csharp
public void Save(string destinationFileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | String | Путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан. |

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
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.lz");
}
```

### См. также

* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Сохраняет lzip-архив в указанный файл назначения.

```csharp
public void Save(FileInfo destination)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | FileInfo | FileInfo, который будет открыт как поток назначения. |

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

## Примеры

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz"));
}
```

### См. также

* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)


