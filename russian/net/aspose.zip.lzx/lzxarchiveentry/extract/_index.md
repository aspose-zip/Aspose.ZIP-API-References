---
title: "LzxArchiveEntry.Extract"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод LzxArchiveEntry. Извлекает запись архива Lzx в файловую систему по пути"
type: docs
weight: 80
url: /ru/net/aspose.zip.lzx/lzxarchiveentry/extract/
---
## Extract(string) {#extract}

Извлекает запись архива Lzx в файловую систему по пути.

```csharp
public FileSystemInfo Extract(string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу, в котором будут храниться распакованные данные. |

### Возвращаемое значение

Экземпляр FileSystemInfoInstance, содержащий извлечённые данные.

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Заголовки архива и служебная информация не были прочитаны. |
| ArgumentNullException | *path* имеет значение null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | *path* пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *path* запрещён. |
| PathTooLongException | Указанный *path*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл по адресу *path* содержит двоеточие (:) в середине строки. |
| InvalidDataException | Несоответствие контрольной суммы заголовков или данных. - или - Архив повреждён. |
| OperationCanceledException | В .NET Framework 4.0 и выше: Выбрасывается, когда извлечение отменяется с помощью предоставленного токена отмены. |
| NotSupportedException | Недопустимый метод сжатия. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается неожиданно. |

## Примеры

```csharp
using (FileStream lzxFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzxArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### См. также

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Извлекает запись в предоставленный поток.

```csharp
public void Extract(Stream destination)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | Stream | Поток назначения. Должен поддерживать запись. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *destination* не поддерживает запись. |
| InvalidDataException | Несоответствие контрольной суммы заголовков или данных. - или - Архив повреждён. |
| ArgumentNullException | Поток назначения равен null. |
| NotSupportedException | Недопустимый метод сжатия. |
| OperationCanceledException | В .NET Framework 4.0 и выше: Выбрасывается, когда извлечение отменяется с помощью предоставленного токена отмены. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается неожиданно. |

### См. также

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)


