---
title: LzmaArchive.Extract
second_title: Aspose.ZIP для справочника API .NET
description: LzmaArchive метод. Извлекает архив lzma в поток.
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
| destination | Stream | Поток для хранения распакованных данных. |

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Заголовки архива и служебная информация не читались. |
| InvalidDataException | Ошибка данных в заголовке или контрольной сумме. |
| ArgumentNullException | Целевой поток равен нулю. |
| ArgumentException | Целевой поток не поддерживает запись. |

### Примеры

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

### Смотрите также

* class [LzmaArchive](../)
* пространство имен [Aspose.Zip.LZMA](../../lzmaarchive/)
* сборка [Aspose.Zip](../../../)

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
| InvalidOperationException | Заголовки архива и служебная информация не читались. |
| SecurityException | У вызывающего абонента нет необходимых разрешений для открытия*fileInfo*. |
| ArgumentException | Путь к файлу пуст или содержит только пробелы. |
| FileNotFoundException | Файл не найден. |
| UnauthorizedAccessException | Путь к файлу доступен только для чтения или является каталогом. |
| ArgumentNullException | *fileInfo* нулевой. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на несопоставленном диске. |
| IOException | Файл уже открыт. |

### Примеры

```csharp
using (FileStream lzmaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzmaArchive(lzmaFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### Смотрите также

* class [LzmaArchive](../)
* пространство имен [Aspose.Zip.LZMA](../../lzmaarchive/)
* сборка [Aspose.Zip](../../../)

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
| InvalidOperationException | Заголовки архива и служебная информация не читались. |
| ArgumentNullException | *path* нулевой. |
| SecurityException | У вызывающего абонента нет необходимого разрешения на доступ. |
| ArgumentException | *path* пуст, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу*path* отказано. |
| PathTooLongException | Указанный*path*, имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. |
| NotSupportedException | Файл в*path* содержит двоеточие (:) в середине строки. |

### Примеры

```csharp
using (FileStream lzmaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzmaArchive(lzmaFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### Смотрите также

* class [LzmaArchive](../)
* пространство имен [Aspose.Zip.LZMA](../../lzmaarchive/)
* сборка [Aspose.Zip](../../../)


