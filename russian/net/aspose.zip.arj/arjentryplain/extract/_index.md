---
title: "ArjEntryPlain.Extract"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод ArjEntryPlain. Извлекает запись в файловую систему по указанному пути"
type: docs
weight: 40
url: /ru/net/aspose.zip.arj/arjentryplain/extract/
---
## Extract(string) {#extract}

Извлекает запись в файловую систему по указанному пути.

```csharp
public FileInfo Extract(string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к целевому файлу. Если файл уже существует, он будет перезаписан. |

### Возвращаемое значение

Информация о файле составного файла.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* равен null или пустой. |
| ObjectDisposedException | Выбрасывается, если архив был освобождён. |
| FileNotFoundException | Файл не найден. |
| InvalidDataException | Несоответствие контрольной суммы заголовков или данных. - или - Архив повреждён. |
| PathTooLongException | Указанный путь, имя файла или их комбинация превышают системно определённую максимальную длину. |
| NotImplementedException | Запись сжата методом 4. |

## Примеры

Извлечь две записи из rar-архива.

```csharp
using (FileStream arjFile = File.Open("archive.arj", FileMode.Open))
{
    using (ArjArchive archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract("first.bin");
        archive.Entries[1].Extract("second.bin");
    }
}
```

### См. также

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Извлекает запись ARJ-архива в файл.

```csharp
public void Extract(FileInfo fileInfo)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo для хранения распакованных данных. |

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Заголовки архива и служебная информация не были прочитаны. |
| SecurityException | У вызывающего нет необходимого разрешения для открытия *fileInfo*. |
| ArgumentException | Путь к файлу пустой или содержит только пробелы. |
| FileNotFoundException | Файл не найден. |
| UnauthorizedAccessException | Путь к файлу доступен только для чтения или является каталогом. |
| ArgumentNullException | *fileInfo* равен null. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| IOException | Файл уже открыт. |
| OperationCanceledException | В .NET Framework 4.0 и выше: Выбрасывается, когда извлечение отменяется с помощью предоставленного токена отмены. |
| ObjectDisposedException | Выбрасывается, если архив был освобождён. |
| InvalidDataException | Несоответствие контрольной суммы заголовков или данных. - или - Архив повреждён. |
| NotImplementedException | Запись сжата методом 4. |

## Примеры

```csharp
using (var arjFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### См. также

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_2}

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
| NotImplementedException | Запись сжата методом 4. |
| OperationCanceledException | В .NET Framework 4.0 и выше: Выбрасывается, когда извлечение отменяется с помощью предоставленного токена отмены. |
| ObjectDisposedException | Выбрасывается, если архив был освобождён. |

### См. также

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)


