---
title: "Lz4Archive.Save"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Lz4Archive метод. Сохраняет lz4 архив в предоставленный поток"
type: docs
weight: 60
url: /ru/net/aspose.zip.lz4/lz4archive/save/
---
## Save(Stream) {#save_1}

Сохраняет архив lz4 в предоставленный поток.

```csharp
public void Save(Stream output)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| output | Stream | Поток назначения. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *output* равен null. |
| ArgumentException | *output* не доступен для записи. |
| InvalidOperationException | Архив подготовлен для извлечения. - или - Источник не был предоставлен. |
| OperationCanceledException | В .NET Framework 4.0 и выше: Выбрасывается, когда сжатие отменяется с помощью предоставленного токена отмены. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примечания

*output* must be seekable.

## Примеры

```csharp
using (FileStream lz4File = File.Open("archive.lz4", FileMode.Create))
{
    using (var archive = new Lz4Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(lz4File);
     }
}
```

### См. также

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Сохраняет архив lz4 в указанный файл назначения.

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
| InvalidOperationException | Архив подготовлен для извлечения. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примеры

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz4"));
}
```

### См. также

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

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
| SecurityException | Вызвавший процесс не имеет необходимого разрешения для доступа. |
| ArgumentException | *destinationFileName* пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *destinationFileName* запрещён. |
| PathTooLongException | Указанный *destinationFileName*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл в *destinationFileName* содержит двоеточие (:) в середине строки. |
| InvalidOperationException | Архив подготовлен для извлечения. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| DirectoryNotFoundException | Указанный путь недействителен (например, он находится на не смонтированном диске). |
| FileNotFoundException | Файл, указанный в *destinationFileName*, не найден. |
| IOException | Во время открытия файла произошла ошибка ввода/вывода. |

## Примеры

```csharp
using (var archive = new LZ4Archive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### См. также

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


