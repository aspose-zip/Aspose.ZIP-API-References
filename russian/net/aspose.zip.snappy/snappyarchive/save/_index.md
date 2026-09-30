---
title: "SnappyArchive.Save"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод SnappyArchive. Сохраняет snappy‑архив в предоставленный поток"
type: docs
weight: 50
url: /ru/net/aspose.zip.snappy/snappyarchive/save/
---
## Save(Stream) {#save_1}

Сохраняет snappy-архив в указанный поток.

```csharp
public void Save(Stream output)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| output | Stream | Поток назначения. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *output* не поддерживает перемотку. |
| ArgumentNullException | *output* равен null. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примечания

*output* must be seekable.

## Примеры

```csharp
using (FileStream snappyFile = File.Open("archive.snappy", FileMode.Create))
{
    using (var archive = new SnappyArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(snappyFile);
     }
}
```

### См. также

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Сохраняет snappy-архив в указанный целевой файл.

```csharp
public void Save(FileInfo destination)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | FileInfo | FileInfo, который будет открыт как поток назначения. |

### Исключения

| исключение | условие |
| --- | --- |
| SecurityException | Вызвавший код не имеет необходимого разрешения для открытия *destination*. |
| ArgumentException | Путь к файлу пустой или содержит только пробелы. |
| FileNotFoundException | Файл не найден. |
| UnauthorizedAccessException | Путь к файлу доступен только для чтения или является каталогом. |
| ArgumentNullException | *destination* равно null. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| IOException | Файл уже открыт. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примеры

```csharp
using (var archive = new SnappyArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.snappy"));
}
```

### См. также

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

Сохраняет snappy-архив в указанный целевой файл.

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
| FileNotFoundException | Указанный файл не найден. |
| IOException | Во время открытия файла произошла ошибка ввода/вывода. |

## Примеры

```csharp
using (var archive = new SnappyArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.snappy");
}
```

### См. также

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)


