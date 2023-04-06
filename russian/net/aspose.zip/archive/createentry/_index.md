---
title: Archive.CreateEntry
second_title: Aspose.ZIP для справочника API .NET
description: Archive метод. Создать одну запись в архиве.
type: docs
weight: 50
url: /ru/net/aspose.zip/archive/createentry/
---
## CreateEntry(string, string, bool, ArchiveEntrySettings) {#createentry_3}

Создать одну запись в архиве.

```csharp
public ArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| path | String | Полное имя нового файла или относительное имя файла для сжатия. |
| openImmediately | Boolean | Истинно, если открыть файл сразу, в противном случае открыть файл при сохранении архива. |
| newEntrySettings | ArchiveEntrySettings | Параметры сжатия и шифрования, используемые для добавленных[`ArchiveEntry`](../../archiveentry/) элемент. |

### Возвращаемое значение

Экземпляр записи ZIP.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* нулевой. |
| SecurityException | У вызывающего абонента нет необходимого разрешения на доступ. |
| ArgumentException | *path* пуст, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу*path* отказано. |
| PathTooLongException | Указанный*path*, имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. |
| NotSupportedException | Файл в*path* содержит двоеточие (:) в середине строки. |

### Примечания

Имя записи устанавливается исключительно в пределах*name* параметр. Имя файла, указанное в*path* параметр не влияет на имя записи.

Если файл открывается сразу с помощью*openImmediately* параметр блокируется до тех пор, пока архив не будет сохранен.

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

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* пространство имен [Aspose.Zip](../../archive/)
* сборка [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings) {#createentry_1}

Создать одну запись в архиве.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| source | Stream | Входной поток для записи. |
| newEntrySettings | ArchiveEntrySettings | Параметры сжатия и шифрования, используемые для добавленных[`ArchiveEntry`](../../archiveentry/) элемент. |

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

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* пространство имен [Aspose.Zip](../../archive/)
* сборка [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool, ArchiveEntrySettings) {#createentry}

Создать одну запись в архиве.

```csharp
public ArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| fileInfo | FileInfo | Метаданные файла для сжатия. |
| openImmediately | Boolean | Истинно, если открыть файл сразу, в противном случае открыть файл при сохранении архива. |
| newEntrySettings | ArchiveEntrySettings | Параметры сжатия и шифрования, используемые для добавленных[`ArchiveEntry`](../../archiveentry/) элемент. |

### Возвращаемое значение

Экземпляр записи ZIP.

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

Составьте архив с записями, зашифрованными разными методами шифрования и паролями.

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

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* пространство имен [Aspose.Zip](../../archive/)
* сборка [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings, FileSystemInfo) {#createentry_2}

Создать одну запись в архиве.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, ArchiveEntrySettings newEntrySettings, 
    FileSystemInfo fileInfo)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| source | Stream | Входной поток для записи. |
| newEntrySettings | ArchiveEntrySettings | Параметры сжатия и шифрования, используемые для добавленных[`ArchiveEntry`](../../archiveentry/) элемент. |
| fileInfo | FileSystemInfo | Метаданные файла или папки для сжатия. |

### Возвращаемое значение

Экземпляр записи ZIP.

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Оба*source* и*fileInfo* являются нулевыми или*source*является нулевым и*fileInfo* обозначает каталог. |

### Примечания

Имя записи устанавливается исключительно в пределах*name* параметр. Имя файла, указанное в*fileInfo* параметр не влияет на имя записи.

*fileInfo* может относиться кDirectoryInfo если запись является каталогом.

### Примеры

Составьте архив с зашифрованной записью.

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

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* пространство имен [Aspose.Zip](../../archive/)
* сборка [Aspose.Zip](../../../)


