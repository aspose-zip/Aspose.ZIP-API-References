---
title: Archive
second_title: Aspose.ZIP для справочника API .NET
description: Инициализирует новый экземплярArchiveaspose.zip/archiveкласс с необязательными настройками для его записей.
type: docs
weight: 10
url: /ru/net/aspose.zip/archive/archive/
---
## Archive(ArchiveEntrySettings) {#constructor}

Инициализирует новый экземпляр[`Archive`](../../archive)класс с необязательными настройками для его записей.

```csharp
public Archive(ArchiveEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| newEntrySettings | ArchiveEntrySettings | Параметры сжатия и шифрования, используемые для вновь добавленных[`ArchiveEntry`](../../archiveentry)items. Если не указано иное, будет использоваться наиболее распространенное сжатие Deflate без шифрования. |

### Примеры

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

### Смотрите также

* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* пространство имен [Aspose.Zip](../../archive)
* сборка [Aspose.Zip](../../../)

---

## Archive(Stream, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_1}

Инициализирует новый экземпляр[`Archive`](../../archive) список записей классов и композиций можно извлечь из архива.

```csharp
public Archive(Stream sourceStream, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. |
| loadOptions | ArchiveLoadOptions | Опции для загрузки существующего архива. |
| newEntrySettings | ArchiveEntrySettings | Параметры сжатия и шифрования, используемые для вновь добавленных[`ArchiveEntry`](../../archiveentry)items. Если не указано иное, будет использоваться наиболее распространенное сжатие Deflate без шифрования. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *sourceStream* не доступен для поиска. |
| InvalidDataException | Заголовок шифрования для AES противоречит методу сжатия WinZip. |

### Примечания

Этот конструктор не распаковывает никакие записи. Видеть[`Open`](../../archiveentry/open) метод распаковки.

### Примеры

В следующем примере извлекается зашифрованный архив, затем распаковывается первая запись в`ПамятьПоток`.

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

### Смотрите также

* class [ArchiveLoadOptions](../../archiveloadoptions)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* пространство имен [Aspose.Zip](../../archive)
* сборка [Aspose.Zip](../../../)

---

## Archive(string, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_2}

Инициализирует новый экземпляр[`Archive`](../../archive) список записей классов и композиций можно извлечь из архива.

```csharp
public Archive(string path, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Полный или относительный путь к файлу архива. |
| loadOptions | ArchiveLoadOptions | Опции для загрузки существующего архива. |
| newEntrySettings | ArchiveEntrySettings | Параметры сжатия и шифрования, используемые для вновь добавленных[`ArchiveEntry`](../../archiveentry)items. Если не указано иное, будет использоваться наиболее распространенное сжатие Deflate без шифрования. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* нулевой. |
| SecurityException | У вызывающего абонента нет необходимого разрешения для доступа |
| ArgumentException | *path* пуст, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу*path* отказано. |
| PathTooLongException | Указанный*path*, имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. |
| NotSupportedException | Файл в*path* содержит двоеточие (:) в середине строки. |

### Примечания

Этот конструктор не распаковывает никакие записи. Видеть[`Open`](../../archiveentry/open) метод распаковки.

### Примеры

В следующем примере извлекается зашифрованный архив, затем распаковывается первая запись в`ПамятьПоток`.

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

### Смотрите также

* class [ArchiveLoadOptions](../../archiveloadoptions)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* пространство имен [Aspose.Zip](../../archive)
* сборка [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
