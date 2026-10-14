---
title: "TarArchive.CreateEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод TarArchive. Создаёт одну запись в архиве"
type: docs
weight: 110
url: /ru/net/aspose.zip.tar/tararchive/createentry/
---
## CreateEntry(string, Stream, FileSystemInfo) {#createentry_1}

Создаёт одну запись внутри архива.

```csharp
public TarEntry CreateEntry(string name, Stream source, FileSystemInfo fileInfo = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| source | Stream | Входной поток для записи. |
| fileInfo | FileSystemInfo | Метаданные файла или папки для сжатия. |

### Возвращаемое значение

Экземпляр записи Tar.

### Исключения

| исключение | условие |
| --- | --- |
| PathTooLongException | *name* слишком длинное для tar согласно стандарту IEEE 1003.1-1998. |
| ArgumentException | Имя файла, как часть *name*, превышает 100 символов. |
| ObjectDisposedException | Архив был освобождён и не может быть использован |

## Примечания

Имя записи задаётся исключительно параметром *name*. Имя файла, указанное в параметре *fileInfo*, не влияет на имя записи.

*fileInfo* can refer to DirectoryInfo if the entry is directory.

## Примеры

```csharp
using (var archive = new TarArchive())
{
   archive.CreateEntry("bytes", new MemoryStream(new byte[] {0x00, 0xFF}));
   archive.Save(tarFile);
}
```

### См. также

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Создаёт одну запись внутри архива.

```csharp
public TarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| fileInfo | FileInfo | Метаданные файла или папки для сжатия. |
| openImmediately | Boolean | True, если файл открывается сразу, иначе файл открывается при сохранении архива. |

### Возвращаемое значение

Экземпляр записи Tar.

### Исключения

| исключение | условие |
| --- | --- |
| PathTooLongException | *name* слишком длинное для tar согласно стандарту IEEE 1003.1-1998. |
| ArgumentException | Имя файла, как часть *name*, превышает 100 символов. |
| ObjectDisposedException | Архив был освобождён и не может быть использован |

## Примечания

Имя записи задаётся исключительно параметром *name*. Имя файла, указанное в параметре *fileInfo*, не влияет на имя записи.

*fileInfo* can refer to DirectoryInfo if the entry is directory.

Если файл открыт сразу с параметром *openImmediately*, он будет заблокирован до освобождения архива.

## Примеры

```csharp
FileInfo fi = new FileInfo("data.bin");
using (var archive = new TarArchive())
{
   archive.CreateEntry("data.bin", fi);
   archive.Save(tarFile);
}
```

### См. также

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Создаёт одну запись внутри архива.

```csharp
public TarEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| path | String | Путь к файлу, который будет сжат. |
| openImmediately | Boolean | True, если файл открывается сразу, иначе файл открывается при сохранении архива. |

### Возвращаемое значение

Экземпляр записи Tar.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* имеет значение null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | *path* пустой, содержит только пробелы или содержит недопустимые символы. - или - Имя файла, как часть *name*, превышает 100 символов. |
| UnauthorizedAccessException | Доступ к файлу *path* запрещён. |
| PathTooLongException | Указанный *path*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. - или - *name* слишком длинное для tar согласно стандарту IEEE 1003.1-1998. |
| NotSupportedException | Файл по адресу *path* содержит двоеточие (:) в середине строки. |
| ObjectDisposedException | Архив был освобождён и не может быть использован |

## Примечания

Имя записи задаётся только параметром *name*. Имя файла, указанное в параметре *path*, не влияет на имя записи.

Если файл открыт сразу с параметром *openImmediately*, он будет заблокирован до освобождения архива.

## Примеры

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save(outputTarFile);
}
```

### См. также

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


