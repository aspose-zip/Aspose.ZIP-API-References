---
title: "SevenZipArchive.CreateEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод SevenZipArchive. Создаёт одну запись в архиве"
type: docs
weight: 50
url: /ru/net/aspose.zip.sevenzip/sevenziparchive/createentry/
---
## CreateEntry(string, FileInfo, bool, SevenZipEntrySettings) {#createentry_1}

Создаёт одну запись внутри архива.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, FileInfo fileInfo, 
    bool openImmediately = false, SevenZipEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| fileInfo | FileInfo | Метаданные файла для сжатия. |
| openImmediately | Boolean | True, если файл открывается сразу, иначе файл открывается при сохранении архива. |
| newEntrySettings | SevenZipEntrySettings | Параметры сжатия и шифрования, используемые для добавленного элемента [`SevenZipArchiveEntry`](../../sevenziparchiveentry/). Индивидуальные параметры сжатия игнорируются при сплошном сжатии, см. [`Solid`](../../../aspose.zip.saving/sevenzipentrysettings/solid/). |

### Возвращаемое значение

Экземпляр записи Seven Zip.

### Исключения

| исключение | условие |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* только для чтения или является каталогом. |
| ArgumentException | *name* равно null или пусто. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| IOException | Файл уже открыт. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примечания

Имя записи задаётся исключительно параметром *name*. Имя файла, указанное в параметре *fileInfo*, не влияет на имя записи.

Если файл открыт сразу с параметром *openImmediately*, он будет заблокирован до сохранения архива.

## Примеры

Создайте архив с записями, зашифрованными разными паролями.

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

### См. также

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings, FileSystemInfo) {#createentry_3}

Создаёт одну запись внутри архива.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings, FileSystemInfo fileInfo)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| source | Stream | Входной поток для записи. |
| newEntrySettings | SevenZipEntrySettings | Параметры сжатия и шифрования, используемые для добавленного элемента [`SevenZipArchiveEntry`](../../sevenziparchiveentry/). Индивидуальные параметры сжатия игнорируются при сплошном сжатии, см. [`Solid`](../../../aspose.zip.saving/sevenzipentrysettings/solid/). |
| fileInfo | FileSystemInfo | Метаданные файла или папки для сжатия. |

### Возвращаемое значение

Экземпляр записи SevenZip.

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Оба *source* и *fileInfo* равны null, либо *source* равен null, а *fileInfo* представляет каталог. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| ArgumentException | *name* равно null или пусто. |

## Примечания

Имя записи задаётся исключительно параметром *name*. Имя файла, указанное в параметре *fileInfo*, не влияет на имя записи.

*fileInfo* can refer to DirectoryInfo if the entry is directory.

## Примеры

Создайте архив с записью, сжатой LZMA2 и зашифрованной.

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

### См. также

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, SevenZipEntrySettings) {#createentry}

Создаёт одну запись внутри архива.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Func<Stream> streamProvider, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| streamProvider | Func`1 | Метод, предоставляющий входной поток для записи. |
| newEntrySettings | SevenZipEntrySettings | Параметры сжатия и шифрования, используемые для добавленного элемента [`SevenZipArchiveEntry`](../../sevenziparchiveentry/). Индивидуальные параметры сжатия игнорируются при сплошном сжатии, см. [`Solid`](../../../aspose.zip.saving/sevenzipentrysettings/solid/). |

### Возвращаемое значение

Экземпляр записи SevenZip.

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Архив создан для распаковки |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| ArgumentException | *name* равно null или пусто. |

## Примеры

Создайте архив с записью, сжатой LZMA2 и зашифрованной.

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", provider, new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1"))); 
        archive.Save(sevenZipFile);
    }
}
```

### См. также

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings) {#createentry_2}

Создаёт одну запись внутри архива.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| source | Stream | Входной поток для записи. |
| newEntrySettings | SevenZipEntrySettings | Параметры сжатия и шифрования, используемые для добавленного элемента [`SevenZipArchiveEntry`](../../sevenziparchiveentry/). Индивидуальные параметры сжатия игнорируются при сплошном сжатии, см. [`Solid`](../../../aspose.zip.saving/sevenzipentrysettings/solid/). |

### Возвращаемое значение

Экземпляр Zip‑записи.

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| ArgumentException | *name* равно null или пусто. |

## Примеры

Создайте 7z‑архив с сжатием LZMA2 и шифрованием всех записей.

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.7z");
}
```

### См. также

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, SevenZipEntrySettings) {#createentry_4}

Создаёт одну запись внутри архива.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| path | String | Полностью квалифицированное имя нового файла или относительное имя файла для сжатия. |
| openImmediately | Boolean | True, если файл открывается сразу, иначе файл открывается при сохранении архива. |
| newEntrySettings | SevenZipEntrySettings | Параметры сжатия и шифрования, используемые для добавленного элемента [`SevenZipArchiveEntry`](../../sevenziparchiveentry/). Индивидуальные параметры сжатия игнорируются при сплошном сжатии, см. [`Solid`](../../../aspose.zip.saving/sevenzipentrysettings/solid/). |

### Возвращаемое значение

Экземпляр Zip‑записи.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* имеет значение null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | *path* пустой, содержит только пробелы или недопустимые символы. - или - *name* равно null или пусто. |
| UnauthorizedAccessException | Доступ к файлу *path* запрещён. |
| PathTooLongException | Указанный *path*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| NotSupportedException | Файл по адресу *path* содержит двоеточие (:) в середине строки. |

## Примечания

Имя записи задаётся только параметром *name*. Имя файла, указанное в параметре *path*, не влияет на имя записи.

Если файл открыт сразу с параметром *openImmediately*, он будет заблокирован до сохранения архива.

## Примеры

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

### См. также

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


