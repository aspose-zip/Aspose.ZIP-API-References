---
title: CpioArchive.CreateEntry
second_title: Aspose.ZIP для справочника API .NET
description: CpioArchive метод. Создать одну запись в архиве.
type: docs
weight: 40
url: /ru/net/aspose.zip.cpio/cpioarchive/createentry/
---
## CreateEntry(string, FileInfo, bool) {#createentry}

Создать одну запись в архиве.

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
| ArgumentNullException | *name* нулевой. |
| ArgumentException | *name* пусто. |
| ArgumentNullException | *fileInfo* нулевой. |

### Примечания

Если файл открывается сразу с помощью*openImmediately*параметр блокируется до тех пор, пока архив не будет удален.

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

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* пространство имен [Aspose.Zip.Cpio](../../cpioarchive/)
* сборка [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Создать одну запись в архиве.

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
| ArgumentNullException | *sourcePath* нулевой. |
| SecurityException | У вызывающего абонента нет необходимого разрешения на доступ. |
| ArgumentException | *sourcePath* пуст, содержит только пробелы или содержит недопустимые символы. - или - Имя файла, как часть*name*, превышает 100 символов. |
| UnauthorizedAccessException | Доступ к файлу*sourcePath* отказано. |
| PathTooLongException | Указанный*sourcePath* , имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. - или -*name* слишком длинный для cpio. |
| NotSupportedException | Файл в*sourcePath* содержит двоеточие (:) в середине строки. |

### Примечания

Имя записи устанавливается исключительно в пределах*name* параметр. Имя файла, указанное в*sourcePath* параметр не влияет на имя записи.

Если файл открывается сразу с помощью*openImmediately*параметр блокируется до тех пор, пока архив не будет удален.

### Примеры

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cpio");
}
```

### Смотрите также

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* пространство имен [Aspose.Zip.Cpio](../../cpioarchive/)
* сборка [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Создать одну запись в архиве.

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
| ArgumentNullException | *name* нулевой. |
| ArgumentNullException | *source* нулевой. |
| ArgumentException | *name* пусто. |

### Примеры

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.cpio");
}
```

### Смотрите также

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* пространство имен [Aspose.Zip.Cpio](../../cpioarchive/)
* сборка [Aspose.Zip](../../../)


