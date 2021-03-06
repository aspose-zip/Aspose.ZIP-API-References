---
title: CreateEntry
second_title: Aspose.ZIP для справочника API .NET
description: Создать одну запись внутри архива.
type: docs
weight: 40
url: /ru/net/aspose.zip.cpio/cpioarchive/createentry/
---
## CreateEntry(string, FileInfo, bool) {#createentry}

Создать одну запись внутри архива.

```csharp
public CpioEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| fileInfo | FileInfo | Метаданные файла или папки для сжатия. |
| openImmediately | Boolean | Истинно, если открыть файл сразу, в противном случае открыть файл при сохранении архива. |

### Возвращаемое значение

Экземпляр записи Cpio.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *имя*равно нулю. |
| ArgumentException | *name*пусто. |
| ArgumentNullException | *fileInfo*равно нулю. |

### Примечания

Если файл открывается сразу с параметром*openImmediately*, он блокируется до удаления архива.

### Примеры

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new CpioArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.cpio");
}
```

### Смотрите также

* class [CpioEntry](../../cpioentry)
* class [CpioArchive](../../cpioarchive)
* пространство имен [Aspose.Zip.Cpio](../../cpioarchive)
* сборка [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Создать одну запись внутри архива.

```csharp
public CpioEntry CreateEntry(string name, string sourcePath, bool openImmediately = false)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| sourcePath | String | Путь к сжимаемому файлу. |
| openImmediately | Boolean | Истинно, если открыть файл сразу, в противном случае открыть файл при сохранении архива. |

### Возвращаемое значение

Экземпляр записи Cpio.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *sourcePath*имеет значение null. |
| SecurityException | У вызывающего абонента нет необходимых прав доступа для доступа |
| ArgumentException | *sourcePath*пуст, содержит только пробелы или недопустимые символы. - или - Имя файла, как часть*name*, превышает 100 символов. |
| UnauthorizedAccessException | Доступ к файлу*sourcePath*запрещен. |
| PathTooLongException | Указанный*sourcePath*, имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. - или -*name*слишком длинное для cpio. |
| NotSupportedException | Файл по адресу*sourcePath*содержит двоеточие (:) в середине строки. |

### Примечания

Имя записи задается исключительно в параметре*name*. Имя файла, указанное в параметре*sourcePath*, не влияет на имя записи.

Если файл открывается сразу с параметром*openImmediately*, он блокируется до удаления архива.

### Примеры

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cpio");
}
```

### Смотрите также

* class [CpioEntry](../../cpioentry)
* class [CpioArchive](../../cpioarchive)
* пространство имен [Aspose.Zip.Cpio](../../cpioarchive)
* сборка [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Создать одну запись внутри архива.

```csharp
public CpioEntry CreateEntry(string name, Stream source)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| source | Stream | Входной поток для записи. |

### Возвращаемое значение

Экземпляр записи Cpio.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *name*равно null. |
| ArgumentNullException | *source*равно null. |
| ArgumentException | *name*пусто. |

### Примеры

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.cpio");
}
```

### Смотрите также

* class [CpioEntry](../../cpioentry)
* class [CpioArchive](../../cpioarchive)
* пространство имен [Aspose.Zip.Cpio](../../cpioarchive)
* сборка [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
