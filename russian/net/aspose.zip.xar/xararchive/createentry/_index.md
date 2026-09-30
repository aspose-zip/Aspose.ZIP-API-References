---
title: "XarArchive.CreateEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод XarArchive. Создаёт одну запись в архиве"
type: docs
weight: 40
url: /ru/net/aspose.zip.xar/xararchive/createentry/
---
## CreateEntry(string, FileInfo, bool, XarCompressionSettings) {#createentry}

Создаёт одну запись внутри архива.

```csharp
public XarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| fileInfo | FileInfo | Метаданные файла или папки для сжатия. |
| openImmediately | Boolean | True, если файл открывается сразу, иначе файл открывается при сохранении архива. |
| compressionSettings | XarCompressionSettings | Настройки сжатия, используемые для добавленного элемента [`XarEntry`](../../xarentry/). |

### Возвращаемое значение

Экземпляр записи Xar.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *name* равен null. |
| ArgumentException | *name* пусто. |
| ArgumentNullException | *fileInfo* равен null. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примечания

Если файл открыт сразу с параметром *openImmediately*, он будет заблокирован до освобождения архива.

## Примеры

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new XarArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.xar");
}
```

### См. также

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, XarCompressionSettings) {#createentry_2}

Создаёт одну запись внутри архива.

```csharp
public XarEntry CreateEntry(string name, string sourcePath, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| sourcePath | String | Путь к файлу, который будет сжат. |
| openImmediately | Boolean | True, если файл открывается сразу, иначе файл открывается при сохранении архива. |
| compressionSettings | XarCompressionSettings | Настройки сжатия, используемые для добавленного элемента [`XarEntry`](../../xarentry/). |

### Возвращаемое значение

Экземпляр записи Xar.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *sourcePath* равен null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | Путь *sourcePath* пуст, содержит только пробелы или содержит недопустимые символы. - or - Имя файла, как часть *name*, превышает 100 символов. |
| UnauthorizedAccessException | Доступ к файлу *sourcePath* запрещён. |
| PathTooLongException | Указанный *sourcePath*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. - или - *name* слишком длинное для xar. |
| NotSupportedException | Файл по пути *sourcePath* содержит двоеточие (:) в середине строки. |
| InvalidOperationException | Невозможно изменить архив xar. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примечания

Имя элемента задаётся исключительно параметром *name*. Имя файла, переданное в параметре *sourcePath*, не влияет на имя элемента.

Если файл открыт сразу с параметром *openImmediately*, он будет заблокирован до освобождения архива.

## Примеры

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.xar");
}
```

### См. также

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, XarCompressionSettings) {#createentry_1}

Создаёт одну запись внутри архива.

```csharp
public XarEntry CreateEntry(string name, Stream source, 
    XarCompressionSettings compressionSettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| source | Stream | Входной поток для записи. |
| compressionSettings | XarCompressionSettings | Настройки сжатия, используемые для добавленного элемента [`XarEntry`](../../xarentry/). |

### Возвращаемое значение

Экземпляр записи Xar.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *name* равен null. |
| ArgumentNullException | *source* равен null. |
| ArgumentException | *name* пусто. |
| InvalidOperationException | Невозможно изменить архив xar. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примеры

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.xar");
}
```

### См. также

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


