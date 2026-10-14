---
title: "CabArchive.CreateEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод CabArchive. Создать одну запись в архиве"
type: docs
weight: 40
url: /ru/net/aspose.zip.cab/cabarchive/createentry/
---
## CreateEntry(string, string, CabEntrySettings) {#createentry_3}

Создаёт одну запись внутри архива.

```csharp
public CabEntry CreateEntry(string name, string path, CabEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| path | String | Полностью квалифицированное имя нового файла или относительное имя файла для сжатия. |
| newEntrySettings | CabEntrySettings | Настройки сжатия и шифрования, используемые для добавленного элемента [`CabEntry`](../../cabentry/) |

### Возвращаемое значение

Экземпляр записи Cab.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* имеет значение null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | *path* пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *path* запрещён. |
| PathTooLongException | Указанный *path*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл по адресу *path* содержит двоеточие (:) в середине строки. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| InvalidOperationException | Архив подготовлен к извлечению и не может добавлять записи. |

## Примечания

Имя записи задаётся только параметром *name*. Имя файла, указанное в параметре *path*, не влияет на имя записи.

## Примеры

```csharp
using (var archive = new CabArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.cab");
}
```

### См. также

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, CabEntrySettings) {#createentry_2}

Создаёт одну запись внутри архива.

```csharp
public CabEntry CreateEntry(string name, Stream source, CabEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| source | Stream | Входной поток для записи. |
| newEntrySettings | CabEntrySettings | Настройки сжатия и шифрования, используемые для добавленного элемента [`CabEntry`](../../cabentry/) |

### Возвращаемое значение

Экземпляр записи Cab.

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| InvalidOperationException | Архив подготовлен к извлечению и не может добавлять записи. |
| ArgumentNullException | *name* равен null. |

## Примеры

```csharp
using (var archive = new CabArchive())
{
    using (var dataStream = new MemoryStream(File.ReadAllBytes("data.bin")))
    {
        archive.CreateEntry("stream-entry.bin", dataStream);
        archive.Save("archive.cab");
    }
}
```

```csharp
using (var archive = new CabArchive())
{     
    var settings = new CabEntrySettings(new CabStoreCompressionSettings());
    archive.CreateEntry("stream-entry.bin", dataStream, settings);
    archive.Save("archive.cab");     
}
```

### См. также

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, CabEntrySettings) {#createentry_1}

Создаёт одну запись внутри архива.

```csharp
public CabEntry CreateEntry(string name, FileInfo fileInfo, 
    CabEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| fileInfo | FileInfo | Метаданные файла для сжатия. |
| newEntrySettings | CabEntrySettings | Настройки сжатия и шифрования, используемые для добавленного элемента [`CabEntry`](../../cabentry/) |

### Возвращаемое значение

Экземпляр записи CAB.

### Исключения

| исключение | условие |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* только для чтения или является каталогом. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| IOException | Файл уже открыт. |
| FileNotFoundException | *fileInfo* представляет файл, который не найден. |
| SecurityException | Вызвавший процесс не имеет необходимого разрешения для доступа к *fileInfo*. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| InvalidOperationException | Архив подготовлен к извлечению и не может добавлять записи. |
| ArgumentNullException | *name* равен null. |

## Примечания

Имя записи задаётся исключительно параметром *name*. Имя файла, указанное в параметре *fileInfo*, не влияет на имя записи.

## Примеры

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{
    var sourceFile = new FileInfo("logs\\log.txt");
    archive.CreateEntry("log.txt", sourceFile);
    archive.Save("archive.cab");
}
```

### См. также

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, CabEntrySettings) {#createentry}

Создаёт одну запись внутри архива.

```csharp
public CabEntry CreateEntry(string name, Func<Stream> streamProvider, 
    CabEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| streamProvider | Func`1 | Метод, предоставляющий входной поток для записи. |
| newEntrySettings | CabEntrySettings | Настройки сжатия и шифрования, используемые для добавленного элемента [`CabEntry`](../../cabentry/) |

### Возвращаемое значение

Экземпляр записи CAB.

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Архив создан для распаковки. - или - Достигнуто ограничение количества файлов. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| ArgumentException | *name* равно null или пусто. |

## Примеры

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{    
    archive.CreateEntry("data.bin", provider);
    archive.Save("archive.cab");
}
```

### См. также

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


