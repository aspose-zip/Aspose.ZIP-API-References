---
title: SnappyArchive.SetSource
second_title: Aspose.ZIP для справочника API .NET
description: SnappyArchive метод. Задает сжатие содержимого внутри архива.
type: docs
weight: 50
url: /ru/net/aspose.zip.snappy/snappyarchive/setsource/
---
## SetSource(Stream) {#setsource_1}

Задает сжатие содержимого внутри архива.

```csharp
public void SetSource(Stream source)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| source | Stream | Входной поток для архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *source* поток недоступен. |

### Примеры

```csharp
using (var archive = new SnappyArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.snappy");
}
```

### Смотрите также

* class [SnappyArchive](../)
* пространство имен [Aspose.Zip.Snappy](../../snappyarchive/)
* сборка [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

Задает сжатие содержимого внутри архива.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo, который будет открыт как входной поток. |

### Исключения

| исключение | условие |
| --- | --- |
| SecurityException | У вызывающего абонента нет необходимых разрешений для открытия*fileInfo*. |
| ArgumentException | Путь к файлу пуст или содержит только пробелы. |
| FileNotFoundException | Файл не найден. |
| UnauthorizedAccessException | Путь к файлу доступен только для чтения или является каталогом. |
| ArgumentNullException | *fileInfo* нулевой. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на несопоставленном диске. |
| IOException | Файл уже открыт. |

### Примеры

```csharp
using (var archive = new SnappyArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.snappy");
}
```

### Смотрите также

* class [SnappyArchive](../)
* пространство имен [Aspose.Zip.Snappy](../../snappyarchive/)
* сборка [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

Задает сжатие содержимого внутри архива.

```csharp
public void SetSource(string sourcePath)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourcePath | String | Путь к файлу, который будет открыт как входной поток. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *sourcePath* нулевой. |
| SecurityException | У вызывающего абонента нет необходимого разрешения на доступ. |
| ArgumentException | *sourcePath* пуст, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу*sourcePath* отказано. |
| PathTooLongException | Указанный*sourcePath*, имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. |
| NotSupportedException | Файл в*sourcePath* содержит двоеточие (:) в середине строки. |

### Примеры

```csharp
using (var archive = new SnappyArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.snappy");
}
```

### Смотрите также

* class [SnappyArchive](../)
* пространство имен [Aspose.Zip.Snappy](../../snappyarchive/)
* сборка [Aspose.Zip](../../../)


