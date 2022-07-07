---
title: CreateEntry
second_title: Aspose.ZIP для справочника API .NET
description: Создать одну запись внутри архива.
type: docs
weight: 50
url: /ru/net/aspose.zip.sevenzip/sevenziparchive/createentry/
---
## CreateEntry(string, FileInfo, bool, SevenZipEntrySettings) {#createentry}

Создать одну запись внутри архива.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, FileInfo fileInfo, 
    bool openImmediately = false, SevenZipEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| fileInfo | FileInfo | Метаданные сжимаемого файла. |
| openImmediately | Boolean | Истинно, если открыть файл сразу, в противном случае открыть файл при сохранении архива. |
| newEntrySettings | SevenZipEntrySettings | Настройки сжатия и шифрования, используемые для добавленного элемента[`SevenZipArchiveEntry`](../../sevenziparchiveentry). |

### Возвращаемое значение

Семь экземпляров записей Zip.

### Исключения

| исключение | условие |
| --- | --- |
| UnauthorizedAccessException | *fileInfo*доступен только для чтения или является каталогом. |
| DirectoryNotFoundException | Указан недопустимый путь, например, на несопоставленном диске. |
| IOException | Файл уже открыт. |

### Примечания

Имя записи задается исключительно в параметре*name*. Имя файла, указанное в параметре*fileInfo*, не влияет на имя записи.

Если файл открывается сразу с параметром*openImmediately*, он блокируется до сохранения архива.

### Примеры

Составить архив с записями, зашифрованными разными паролями.

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

Создать одну запись внутри архива.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings, FileSystemInfo fileInfo)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| source | Stream | Входной поток для записи. |
| newEntrySettings | SevenZipEntrySettings | Настройки сжатия и шифрования, используемые для добавленного элемента[`SevenZipArchiveEntry`](../../sevenziparchiveentry). |
| fileInfo | FileSystemInfo | Метаданные файла или папки для сжатия. |

### Возвращаемое значение

Экземпляр записи SevenZip.

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Оба*source*и*fileInfo*имеют значение null или*source*имеют значение null, а*fileInfo*обозначает каталог. |

### Примечания

Имя записи задается исключительно в параметре*name*. Имя файла, указанное в параметре*fileInfo*, не влияет на имя записи.

*fileInfo*может ссылаться наDirectoryInfoесли запись является каталогом.

### Примеры

Составить архив со сжатой зашифрованной записью LZMA2.

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

Создать одну запись внутри архива.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| source | Stream | Входной поток для записи. |
| newEntrySettings | SevenZipEntrySettings | Настройки сжатия и шифрования, используемые для добавленного элемента[`SevenZipArchiveEntry`](../../sevenziparchiveentry). |

### Возвращаемое значение

Экземпляр записи ZIP.

### Примеры

Составить 7z архив со сжатием LZMA2 и шифрованием всех записей.

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

Создать одну запись внутри архива.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| path | String | Полное имя нового файла или относительное имя файла для сжатия. |
| openImmediately | Boolean | Истинно, если открыть файл сразу, в противном случае открыть файл при сохранении архива. |
| newEntrySettings | SevenZipEntrySettings | Настройки сжатия и шифрования, используемые для добавленного элемента[`SevenZipArchiveEntry`](../../sevenziparchiveentry). |

### Возвращаемое значение

Экземпляр записи ZIP.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path*is нулевой. |
| SecurityException | У вызывающего абонента нет необходимых прав доступа для доступа |
| ArgumentException | *path*пуст, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу*path*запрещен. |
| PathTooLongException | Указанный*path*, имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. |
| NotSupportedException | Файл по адресу*path*содержит двоеточие (:) в середине строки. |

### Примечания

Имя записи задается исключительно в параметре*name*. Имя файла, указанное в параметре*path*, не влияет на имя записи.

Если файл открывается сразу с параметром*openImmediately*, он блокируется до сохранения архива.

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
