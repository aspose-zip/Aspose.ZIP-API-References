---
title: "Archive.CreateEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод Archive. Создаёт одну запись в архиве."
type: docs
weight: 60
url: /ru/net/aspose.zip/archive/createentry/
---
## CreateEntry(string, string, bool, ArchiveEntrySettings) {#createentry_4}

Создаёт одну запись внутри архива.

```csharp
public ArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| path | String | Полностью квалифицированное имя нового файла или относительное имя файла для сжатия. |
| openImmediately | Boolean | True, если файл открывается сразу, иначе файл открывается при сохранении архива. |
| newEntrySettings | ArchiveEntrySettings | Настройки сжатия и шифрования, используемые для добавленного элемента [`ArchiveEntry`](../../archiveentry/). |

### Возвращаемое значение

Экземпляр Zip‑записи.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* имеет значение null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | *path* пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *path* запрещён. |
| PathTooLongException | Указанный *path*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл по адресу *path* содержит двоеточие (:) в середине строки. |
| ObjectDisposedException | Выбрасывается, если архив был освобождён. |

## Примечания

Имя записи задаётся только параметром *name*. Имя файла, указанное в параметре *path*, не влияет на имя записи.

Если файл открыт сразу с параметром *openImmediately*, он будет заблокирован до сохранения архива.

## Примеры

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

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings) {#createentry_2}

Создаёт одну запись внутри архива.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| source | Stream | Входной поток для записи. |
| newEntrySettings | ArchiveEntrySettings | Настройки сжатия и шифрования, используемые для добавленного элемента [`ArchiveEntry`](../../archiveentry/). |

### Возвращаемое значение

Экземпляр Zip‑записи.

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Выбрасывается, если архив был освобождён. |
| InvalidOperationException | Выбрасывается, когда добавление записи недопустимо из‑за текущего состояния архива. |

## Примеры

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.zip");
}
```

### См. также

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool, ArchiveEntrySettings) {#createentry_1}

Создаёт одну запись внутри архива.

```csharp
public ArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| fileInfo | FileInfo | Метаданные файла для сжатия. |
| openImmediately | Boolean | True, если файл открывается сразу, иначе файл открывается при сохранении архива. |
| newEntrySettings | ArchiveEntrySettings | Настройки сжатия и шифрования, используемые для добавленного элемента [`ArchiveEntry`](../../archiveentry/). |

### Возвращаемое значение

Экземпляр Zip‑записи.

### Исключения

| исключение | условие |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* только для чтения или является каталогом. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| IOException | Файл уже открыт. |
| ObjectDisposedException | Выбрасывается, если архив был освобождён. |
| InvalidOperationException | Выбрасывается, когда добавление записи недопустимо из‑за текущего состояния архива. |

## Примечания

Имя записи задаётся исключительно параметром *name*. Имя файла, указанное в параметре *fileInfo*, не влияет на имя записи.

Если файл открыт сразу с параметром *openImmediately*, он будет заблокирован до сохранения архива.

## Примеры

Создайте архив с записями, зашифрованными разными методами шифрования и паролями.

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

### См. также

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings, FileSystemInfo) {#createentry_3}

Создаёт одну запись внутри архива.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, ArchiveEntrySettings newEntrySettings, 
    FileSystemInfo fileInfo)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| source | Stream | Входной поток для записи. |
| newEntrySettings | ArchiveEntrySettings | Настройки сжатия и шифрования, используемые для добавленного элемента [`ArchiveEntry`](../../archiveentry/). |
| fileInfo | FileSystemInfo | Метаданные файла или папки для сжатия. |

### Возвращаемое значение

Экземпляр Zip‑записи.

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Оба *source* и *fileInfo* равны null, либо *source* равен null, а *fileInfo* представляет каталог. |
| ObjectDisposedException | Выбрасывается, если архив был освобождён. |

## Примечания

Имя записи задаётся исключительно параметром *name*. Имя файла, указанное в параметре *fileInfo*, не влияет на имя записи.

*fileInfo* can refer to DirectoryInfo if the entry is directory.

## Примеры

Создайте архив с зашифрованной записью.

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

### См. также

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, ArchiveEntrySettings) {#createentry}

Создаёт одну запись внутри архива.

```csharp
public ArchiveEntry CreateEntry(string name, Func<Stream> streamProvider, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| streamProvider | Func`1 | Метод, предоставляющий входной поток для записи. |
| newEntrySettings | ArchiveEntrySettings | Настройки сжатия и шифрования, используемые для добавленного элемента [`ArchiveEntry`](../../archiveentry/). |

### Возвращаемое значение

Экземпляр Zip‑записи.

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Выбрасывается, если архив был освобождён. |
| ArgumentException | Выбрасывается, когда *name* равен null или пуст, либо *streamProvider* равен null. |
| InvalidOperationException | Выбрасывается, когда архив не поддерживает добавление записей. |

## Примечания

Этот метод предназначен для .NET Framework 4.0 и выше, а также для .NET Standard 2.0 и выше.

## Примеры

Создайте архив с зашифрованной записью.

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", provider, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")))); 
        archive.Save(zipFile);
    }
}
```

### См. также

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


