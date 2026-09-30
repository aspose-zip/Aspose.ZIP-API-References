---
title: "SnappyArchive.SetSource"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод SnappyArchive. Устанавливает содержимое, которое будет сжато в архиве"
type: docs
weight: 60
url: /ru/net/aspose.zip.snappy/snappyarchive/setsource/
---
## SetSource(Stream) {#setsource_1}

Устанавливает содержимое, которое будет сжато в архиве.

```csharp
public void SetSource(Stream source)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| source | Stream | Входной поток для архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | Поток *source* не поддерживает поиск. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примеры

```csharp
using (var archive = new SnappyArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.snappy");
}
```

### См. также

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

Устанавливает содержимое, которое будет сжато в архиве.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo, который будет открыт как входной поток. |

### Исключения

| исключение | условие |
| --- | --- |
| SecurityException | У вызывающего нет необходимого разрешения для открытия *fileInfo*. |
| ArgumentException | Путь к файлу пустой или содержит только пробелы. |
| FileNotFoundException | Файл не найден. |
| UnauthorizedAccessException | Путь к файлу доступен только для чтения или является каталогом. |
| ArgumentNullException | *fileInfo* равен null. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| IOException | Файл уже открыт. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примеры

```csharp
using (var archive = new SnappyArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.snappy");
}
```

### См. также

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

Устанавливает содержимое, которое будет сжато в архиве.

```csharp
public void SetSource(string sourcePath)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourcePath | String | Путь к файлу, который будет открыт как входной поток. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *sourcePath* равен null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | Значение *sourcePath* пусто, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *sourcePath* запрещён. |
| PathTooLongException | Указанный *sourcePath*, имя файла или оба превышают системно‑определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл по пути *sourcePath* содержит двоеточие (:) в середине строки. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| FileNotFoundException | Файл не найден. |

## Примеры

```csharp
using (var archive = new SnappyArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.snappy");
}
```

### См. также

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)


