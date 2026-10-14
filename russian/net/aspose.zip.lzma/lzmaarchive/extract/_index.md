---
title: "LzmaArchive.Extract"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод LzmaArchive. Извлекает lzma архив в поток"
type: docs
weight: 30
url: /ru/net/aspose.zip.lzma/lzmaarchive/extract/
---
## Extract(Stream) {#extract_1}

Извлекает архив lzma в поток.

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
| InvalidDataException | Архив повреждён. |
| ArgumentNullException | Поток назначения равен null. |
| ArgumentException | Поток назначения не поддерживает запись. |

## Примеры

```csharp
using (FileStream sourceLzmaFile = File.Open(sourceFileName, FileMode.Open))
{
   using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
   {
       using (var archive = new LzmaArchive(sourceLzmaFile))
       {
           archive.Extract(extractedFile);
       }
   }
}
```

### См. также

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract}

Извлекает архив lzma в файл.

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
| InvalidDataException | Архив повреждён. |

## Примеры

```csharp
using (FileStream lzmaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzmaArchive(lzmaFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### См. также

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(string) {#extract_2}

Извлекает архив lzma в файл по пути.

```csharp
public void Extract(string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу, в котором будут храниться распакованные данные. |

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
| InvalidDataException | Архив повреждён. |
| FileNotFoundException | Файл не найден. |

## Примеры

```csharp
using (FileStream lzmaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzmaArchive(lzmaFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### См. также

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)


