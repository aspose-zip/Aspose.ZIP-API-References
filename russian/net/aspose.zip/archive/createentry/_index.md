---
title: CreateEntry
second_title: Aspose.ZIP для справочника API .NET
description: Создать одну запись внутри архива.
type: docs
weight: 50
url: /ru/net/aspose.zip/archive/createentry/
---
## CreateEntry(string, string, bool, ArchiveEntrySettings) {#createentry_3}

Создать одну запись внутри архива.

```csharp
public ArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| path | String | Полное имя нового файла или относительное имя файла для сжатия. |
| openImmediately | Boolean | Истинно, если открыть файл сразу, в противном случае открыть файл при сохранении архива. |
| newEntrySettings | ArchiveEntrySettings | Настройки сжатия и шифрования, используемые для добавленного элемента[`ArchiveEntry`](../../archiveentry). |

### Возвращаемое значение

Экземпляр записи ZIP.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path*равно null. |
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

* class [ArchiveEntry](../../archiveentry)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* пространство имен [Aspose.Zip](../../archive)
* сборка [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings) {#createentry_1}

Создать одну запись внутри архива.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| source | Stream | Входной поток для записи. |
| newEntrySettings | ArchiveEntrySettings | Настройки сжатия и шифрования, используемые для добавленного элемента[`ArchiveEntry`](../../archiveentry). |

### Возвращаемое значение

Экземпляр записи ZIP.

### Примеры

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.zip");
}
```

### Смотрите также

* class [ArchiveEntry](../../archiveentry)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* пространство имен [Aspose.Zip](../../archive)
* сборка [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool, ArchiveEntrySettings) {#createentry}

Создать одну запись внутри архива.

```csharp
public ArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| fileInfo | FileInfo | Метаданные сжимаемого файла. |
| openImmediately | Boolean | Истинно, если открыть файл сразу, в противном случае открыть файл при сохранении архива. |
| newEntrySettings | ArchiveEntrySettings | Настройки сжатия и шифрования, используемые для добавленного элемента[`ArchiveEntry`](../../archiveentry). |

### Возвращаемое значение

Экземпляр записи ZIP.

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

Составьте архив с записями, зашифрованными разными методами шифрования и паролями каждая.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
        archive.CreateEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass2", EncryptionMethod.AES128)));
        archive.CreateEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass3", EncryptionMethod.AES256)));
        archive.Save(zipFile);
    }
}
```

### Смотрите также

* class [ArchiveEntry](../../archiveentry)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* пространство имен [Aspose.Zip](../../archive)
* сборка [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings, FileSystemInfo) {#createentry_2}

Создать одну запись внутри архива.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, ArchiveEntrySettings newEntrySettings, 
    FileSystemInfo fileInfo)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| source | Stream | Входной поток для записи. |
| newEntrySettings | ArchiveEntrySettings | Настройки сжатия и шифрования, используемые для добавленного элемента[`ArchiveEntry`](../../archiveentry). |
| fileInfo | FileSystemInfo | Метаданные файла или папки для сжатия. |

### Возвращаемое значение

Экземпляр записи ZIP.

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Оба*source*и*fileInfo*имеют значение null или*source*имеют значение null, а*fileInfo*обозначает каталог. |

### Примечания

Имя записи задается исключительно в параметре*name*. Имя файла, указанное в параметре*fileInfo*, не влияет на имя записи.

*fileInfo*может ссылаться наDirectoryInfoесли запись является каталогом.

### Примеры

Составить архив с зашифрованной записью.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF} ), new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")), new FileInfo("data1.bin")); 
        archive.Save(zipFile);
    }
}
```

### Смотрите также

* class [ArchiveEntry](../../archiveentry)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* пространство имен [Aspose.Zip](../../archive)
* сборка [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
