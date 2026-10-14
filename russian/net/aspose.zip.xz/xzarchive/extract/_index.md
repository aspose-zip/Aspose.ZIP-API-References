---
title: "XzArchive.Extract"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод XzArchive. Извлекает xz‑архив в поток"
type: docs
weight: 40
url: /ru/net/aspose.zip.xz/xzarchive/extract/
---
## Extract(Stream) {#extract_2}

Извлекает архив xz в поток.

```csharp
public void Extract(Stream destination)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | Stream | Поток для хранения распакованных данных. |

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| InvalidOperationException | Заголовки архива и служебная информация не были прочитаны. |
| OperationCanceledException | В .NET Framework 4.0 и выше: Выбрасывается, когда извлечение отменяется с помощью предоставленного токена отмены. |

## Примеры

```csharp
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new XzArchive(xzFile))
        {
            archive.Extract(extractedFile);
        }
    }
}
```

### См. также

* class [XzArchive](../)
* namespace [Aspose.Zip.Xz](../../xzarchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Извлекает архив xz в файл.

```csharp
public void Extract(FileInfo fileInfo)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo для хранения распакованных данных. |

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| InvalidOperationException | Заголовки архива и служебная информация не были прочитаны. |
| SecurityException | У вызывающего нет необходимого разрешения для открытия *fileInfo*. |
| ArgumentException | Путь к файлу пустой или содержит только пробелы. |
| FileNotFoundException | Файл не найден. |
| UnauthorizedAccessException | Путь к файлу доступен только для чтения или является каталогом. |
| ArgumentNullException | *fileInfo* равен null. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| IOException | Файл уже открыт. |
| OperationCanceledException | В .NET Framework 4.0 и выше: Выбрасывается, когда извлечение отменяется с помощью предоставленного токена отмены. |
| InvalidDataException | Данные недействительны или повреждены. |

## Примеры

```csharp
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new XzArchive(xzFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### См. также

* class [XzArchive](../)
* namespace [Aspose.Zip.Xz](../../xzarchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Извлекает архив xz в файл по пути.

```csharp
public FileInfo Extract(string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу, в котором будут храниться распакованные данные. |

### Возвращаемое значение

Экземпляр FileInfo, содержащий извлечённые данные.

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| InvalidOperationException | Заголовки архива и служебная информация не были прочитаны. |
| ArgumentNullException | *path* имеет значение null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | *path* пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *path* запрещён. |
| PathTooLongException | Указанный *path*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл по адресу *path* содержит двоеточие (:) в середине строки. |
| FileNotFoundException | Файл не найден. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| IOException | Файл уже открыт. |
| OperationCanceledException | В .NET Framework 4.0 и выше: Выбрасывается, когда извлечение отменяется с помощью предоставленного токена отмены. |
| InvalidDataException | Данные недействительны или повреждены. |

## Примеры

```csharp
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new XzArchive(xzFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### См. также

* class [XzArchive](../)
* namespace [Aspose.Zip.Xz](../../xzarchive/)
* assembly [Aspose.Zip](../../../)


