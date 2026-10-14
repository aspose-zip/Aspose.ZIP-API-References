---
title: "ZstandardArchive.SetSource"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод ZstandardArchive. Устанавливает содержимое, которое будет сжато в архиве"
type: docs
weight: 70
url: /ru/net/aspose.zip.zstandard/zstandardarchive/setsource/
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
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примеры

```csharp
using (var archive = new ZstandardArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.zst");
}
```

### См. также

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

Устанавливает содержимое, которое будет сжато в архиве.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileInfo | FileInfo | Ссылка на файл, который будет сжат. |

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примеры

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.zst");
}
```

### См. также

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

Устанавливает содержимое, которое будет сжато в архиве.

```csharp
public void SetSource(string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу, который будет сжат. |

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| ArgumentNullException | *path* имеет значение null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | *path* пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *path* запрещён. |
| PathTooLongException | Указанный *path*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл по адресу *path* содержит двоеточие (:) в середине строки. |

## Примеры

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.zst");
}
```

### См. также

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


