---
title: SnappyArchive.Extract
second_title: Aspose.ZIP для справочника API .NET
description: SnappyArchive метод. Извлекает архив snappy в поток.
type: docs
weight: 30
url: /ru/net/aspose.zip.snappy/snappyarchive/extract/
---
## Extract(Stream) {#extract_2}

Извлекает архив snappy в поток.

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
using (FileStream sourceSnappyFile = File.Open(sourceFileName, FileMode.Open))
{
   using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
   {
       using (var archive = new SnappyArchive(sourceSnappyFile))
       {
           archive.Extract(extractedFile);
       }
   }
}
```

### Смотрите также

* class [SnappyArchive](../)
* пространство имен [Aspose.Zip.Snappy](../../snappyarchive/)
* сборка [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Извлекает архив snappy в файл.

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
using (FileStream snappyFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new SnappyArchive(snappyFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### Смотрите также

* class [SnappyArchive](../)
* пространство имен [Aspose.Zip.Snappy](../../snappyarchive/)
* сборка [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Извлекает архив snappy в файл по пути.

```csharp
public FileInfo Extract(string path)
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
using (FileStream snappyFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new SnappyArchive(snappyFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### Смотрите также

* class [SnappyArchive](../)
* пространство имен [Aspose.Zip.Snappy](../../snappyarchive/)
* сборка [Aspose.Zip](../../../)


