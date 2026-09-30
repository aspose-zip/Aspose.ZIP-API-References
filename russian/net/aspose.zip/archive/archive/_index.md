---
title: "Archive.Archive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор Archive. Инициализирует новый экземпляр класса Archive с необязательными настройками для его элементов."
type: docs
weight: 10
url: /ru/net/aspose.zip/archive/archive/
---
## Archive(ArchiveEntrySettings) {#constructor}

Инициализирует новый экземпляр класса [`Archive`](../) с необязательными настройками для его элементов.

```csharp
public Archive(ArchiveEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| newEntrySettings | ArchiveEntrySettings | Настройки сжатия и шифрования, используемые для вновь добавленных элементов [`ArchiveEntry`](../../archiveentry/). Если не указано, будет использовано наиболее распространённое сжатие Deflate без шифрования. |

## Примеры

В следующем примере показано, как сжать один файл с настройками по умолчанию.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### См. также

* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## Archive(Stream, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_1}

Инициализирует новый экземпляр класса [`Archive`](../) и формирует список элементов, который может быть извлечён из архива.

```csharp
public Archive(Stream sourceStream, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. |
| loadOptions | ArchiveLoadOptions | Параметры загрузки существующего архива. |
| newEntrySettings | ArchiveEntrySettings | Настройки сжатия и шифрования, используемые для вновь добавленных элементов [`ArchiveEntry`](../../archiveentry/). Если не указано, будет использовано наиболее распространённое сжатие Deflate без шифрования. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *sourceStream* не поддерживает перемещение, если загружен без установленного [`ForwardOnly`](../../archiveloadoptions/forwardonly/). |
| InvalidDataException | Заголовок шифрования AES противоречит методу сжатия WinZip. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| NotSupportedException | Выбрасывается, когда архив загружается из потока только для чтения в режиме оценки. |

## Примечания

Этот конструктор не распаковывает ни один элемент. См. метод [`Open`](../../archiveentry/open/) для распаковки.

## Примеры

В следующем примере извлекается зашифрованный архив, затем первая запись распаковывается в `MemoryStream`.

```csharp
var fs = File.OpenRead("encrypted.zip");
var extracted = new MemoryStream();
using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### См. также

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## Archive(string, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_2}

Инициализирует новый экземпляр класса [`Archive`](../) и формирует список элементов, который может быть извлечён из архива.

```csharp
public Archive(string path, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Полный или относительный путь к файлу архива. |
| loadOptions | ArchiveLoadOptions | Параметры загрузки существующего архива. |
| newEntrySettings | ArchiveEntrySettings | Настройки сжатия и шифрования, используемые для вновь добавленных элементов [`ArchiveEntry`](../../archiveentry/). Если не указано, будет использовано наиболее распространённое сжатие Deflate без шифрования. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* имеет значение null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | *path* пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *path* запрещён. |
| PathTooLongException | Указанный *path*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл по адресу *path* содержит двоеточие (:) в середине строки. |
| FileNotFoundException | Файл не найден. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| IOException | Файл уже открыт. |
| InvalidDataException | Файл повреждён. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |

## Примечания

Этот конструктор не распаковывает ни один элемент. См. метод [`Open`](../../archiveentry/open/) для распаковки.

## Примеры

В следующем примере извлекается зашифрованный архив, затем первая запись распаковывается в `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (Archive archive = new Archive("encrypted.zip", new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### См. также

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## Archive(string, string[], ArchiveLoadOptions) {#constructor_3}

Инициализирует новый экземпляр класса [`Archive`](../) из многотомного ZIP-архива и формирует список элементов, который может быть извлечён из архива.

```csharp
public Archive(string mainSegment, string[] segmentsInOrder, ArchiveLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| mainSegment | String | Путь к последнему сегменту многотомного архива с центральным каталогом. |
| segmentsInOrder | String[] | Пути к каждому сегменту, кроме последнего, многотомного zip-архива в правильном порядке. |
| loadOptions | ArchiveLoadOptions | Параметры загрузки существующего архива. |

### Исключения

| исключение | условие |
| --- | --- |
| EndOfStreamException | Не удалось загрузить заголовки ZIP, потому что предоставленные файлы повреждены. |
| DirectoryNotFoundException | Указанный путь недействителен (например, он находится на не смонтированном диске). |
| FileNotFoundException | Файл, указанный в пути, не найден. |
| IOException | Во время открытия файла произошла ошибка ввода/вывода. |
| PathTooLongException | Указанный путь, имя файла или их комбинация превышают системно определённую максимальную длину. |
| UnauthorizedAccessException | Указанный путь является каталогом. -или- У вызывающего отсутствует необходимое разрешение. |

## Примеры

Этот пример извлекает в каталог архив из трёх сегментов.

```csharp
using (Archive a = new Archive("archive.zip", new string[] { "archive.z01", "archive.z02" }))
{
    a.ExtractToDirectory("destination");
}
```

### См. также

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


