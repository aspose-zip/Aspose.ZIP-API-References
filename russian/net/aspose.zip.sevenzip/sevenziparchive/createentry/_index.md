---
title: CreateEntry
second_title: Aspose.ZIP для справочника API .NET
description: Создать одну запись в архиве.
type: docs
weight: 50
url: /ru/net/aspose.zip.sevenzip/sevenziparchive/createentry/
---
## CreateEntry(string, FileInfo, bool, SevenZipEntrySettings) {#createentry}

Создать одну запись в архиве.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, FileInfo fileInfo, 
    bool openImmediately = false, SevenZipEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| fileInfo | FileInfo | Метаданные файла для сжатия. |
| openImmediately | Boolean | Истинно, если открыть файл сразу, в противном случае открыть файл при сохранении архива. |
| newEntrySettings | SevenZipEntrySettings | Параметры сжатия и шифрования, используемые для добавленных[`SevenZipArchiveEntry`](../../sevenziparchiveentry) вещь. |

### Возвращаемое значение

Экземпляр записи Seven Zip.

### Исключения

| исключение | условие |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* доступен только для чтения или является каталогом. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на несопоставленном диске. |
| IOException | Файл уже открыт. |

### Примечания

Имя записи устанавливается исключительно в пределах*name* параметр. Имя файла, указанное в*fileInfo* параметр не влияет на имя записи.

Если файл открывается сразу с помощью*openImmediately* параметр блокируется до тех пор, пока архив не будет сохранен.

### Примеры

Составьте архив с записями, зашифрованными разными паролями.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
        archive.CreateEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
        archive.CreateEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
        archive.Save(sevenZipFile);
    }
}
```

### Смотрите также

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* пространство имен [Aspose.Zip.SevenZip](../../sevenziparchive)
* сборка [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings, FileSystemInfo) {#createentry_2}

Создать одну запись в архиве.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings, FileSystemInfo fileInfo)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| source | Stream | Входной поток для записи. |
| newEntrySettings | SevenZipEntrySettings | Параметры сжатия и шифрования, используемые для добавленных[`SevenZipArchiveEntry`](../../sevenziparchiveentry) вещь. |
| fileInfo | FileSystemInfo | Метаданные файла или папки для сжатия. |

### Возвращаемое значение

Экземпляр записи SevenZip.

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Оба*source* а также*fileInfo* являются нулевыми или*source* является нулевым и*fileInfo* обозначает каталог. |

### Примечания

Имя записи устанавливается исключительно в пределах*name* параметр. Имя файла, указанное в*fileInfo* параметр не влияет на имя записи.

*fileInfo* может относиться кDirectoryInfo если запись является каталогом.

### Примеры

Составьте архив со сжатой зашифрованной записью LZMA2.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF}), new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1")), new FileInfo("data1.bin")); 
        archive.Save(sevenZipFile);
    }
}
```

### Смотрите также

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* пространство имен [Aspose.Zip.SevenZip](../../sevenziparchive)
* сборка [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings) {#createentry_1}

Создать одну запись в архиве.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| source | Stream | Входной поток для записи. |
| newEntrySettings | SevenZipEntrySettings | Параметры сжатия и шифрования, используемые для добавленных[`SevenZipArchiveEntry`](../../sevenziparchiveentry) вещь. |

### Возвращаемое значение

Экземпляр записи ZIP.

### Примеры

Составьте архив 7z со сжатием LZMA2 и шифрованием всех записей.

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.7z");
}
```

### Смотрите также

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* пространство имен [Aspose.Zip.SevenZip](../../sevenziparchive)
* сборка [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, SevenZipEntrySettings) {#createentry_3}

Создать одну запись в архиве.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| path | String | Полное имя нового файла или относительное имя файла для сжатия. |
| openImmediately | Boolean | Истинно, если открыть файл сразу, в противном случае открыть файл при сохранении архива. |
| newEntrySettings | SevenZipEntrySettings | Параметры сжатия и шифрования, используемые для добавленных[`SevenZipArchiveEntry`](../../sevenziparchiveentry) вещь. |

### Возвращаемое значение

Экземпляр записи ZIP.

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

Имя записи устанавливается исключительно в пределах*name* параметр. Имя файла, указанное в*path* параметр не влияет на имя записи.

Если файл открывается сразу с помощью*openImmediately* параметр блокируется до тех пор, пока архив не будет сохранен.

### Примеры

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings())))
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### Смотрите также

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* пространство имен [Aspose.Zip.SevenZip](../../sevenziparchive)
* сборка [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
