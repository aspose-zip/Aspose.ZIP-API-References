---
title: LzipArchive.Save
second_title: Aspose.ZIP для справочника API .NET
description: LzipArchive метод. Сохраняет lzipархив в указанный поток.
type: docs
weight: 50
url: /ru/net/aspose.zip.lzip/lziparchive/save/
---
## Save(Stream) {#save_1}

Сохраняет lzip-архив в указанный поток.

```csharp
public void Save(Stream outputStream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| outputStream | Stream | Целевой поток. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *outputStream* не поддерживает поиск. |
| ArgumentNullException | *outputStream* нулевой. |

### Примечания

*outputStream* должен быть доступен для поиска.

### Примеры

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

### Смотрите также

* class [LzipArchive](../)
* пространство имен [Aspose.Zip.Lzip](../../lziparchive/)
* сборка [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

Сохраняет архив lzip в указанный файл назначения.

```csharp
public void Save(string destinationFileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | String | Путь создаваемого архива. Если указанное имя файла указывает на существующий файл, он будет перезаписан. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *destinationFileName* нулевой. |
| SecurityException | У вызывающего абонента нет необходимого разрешения на доступ. |
| ArgumentException | *destinationFileName* пуст, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу*destinationFileName* отказано. |
| PathTooLongException | Указанный*destinationFileName*, имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. |
| NotSupportedException | Файл в*destinationFileName* содержит двоеточие (:) в середине строки. |

### Примеры

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.lz");
}
```

### Смотрите также

* class [LzipArchive](../)
* пространство имен [Aspose.Zip.Lzip](../../lziparchive/)
* сборка [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Сохраняет архив lzip в указанный файл назначения.

```csharp
public void Save(FileInfo destination)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destination | FileInfo | FileInfo, который будет открыт как поток назначения. |

### Исключения

| исключение | условие |
| --- | --- |
| SecurityException | У вызывающего абонента нет необходимых разрешений для открытия*destination*. |
| ArgumentException | Путь к файлу пуст или содержит только пробелы. |
| FileNotFoundException | Файл не найден. |
| UnauthorizedAccessException | Путь к файлу доступен только для чтения или является каталогом. |
| ArgumentNullException | *destination* нулевой. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на несопоставленном диске. |
| IOException | Файл уже открыт. |

### Примеры

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz"));
}
```

### Смотрите также

* class [LzipArchive](../)
* пространство имен [Aspose.Zip.Lzip](../../lziparchive/)
* сборка [Aspose.Zip](../../../)


