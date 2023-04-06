---
title: TarArchive.CreateEntry
second_title: Aspose.ZIP для справочника API .NET
description: TarArchive метод. Создать одну запись в архиве.
type: docs
weight: 80
url: /ru/net/aspose.zip.tar/tararchive/createentry/
---
## CreateEntry(string, Stream, FileSystemInfo) {#createentry_1}

Создать одну запись в архиве.

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
| PathTooLongException | *name* слишком длинный для tar по стандарту IEEE 1003.1-1998. |
| ArgumentException | Имя файла, как часть*name*, превышает 100 символов. |

### Примечания

Имя записи устанавливается исключительно в пределах*name* параметр. Имя файла, указанное в*fileInfo* параметр не влияет на имя записи.

*fileInfo* может относиться кDirectoryInfo если запись является каталогом.

### Примеры

```csharp
using (var archive = new TarArchive())
{
   archive.CreateEntry("bytes", new MemoryStream(new byte[] {0x00, 0xFF}));
   archive.Save(tarFile);
}
```

### Смотрите также

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* пространство имен [Aspose.Zip.Tar](../../tararchive/)
* сборка [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Создать одну запись в архиве.

```csharp
public TarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| fileInfo | FileInfo | Метаданные файла или папки для сжатия. |
| openImmediately | Boolean | Истинно, если открыть файл сразу, в противном случае открыть файл при сохранении архива. |

### Возвращаемое значение

Экземпляр записи Tar.

### Исключения

| исключение | условие |
| --- | --- |
| PathTooLongException | *name* слишком длинный для tar по стандарту IEEE 1003.1-1998. |
| ArgumentException | Имя файла, как часть*name*, превышает 100 символов. |

### Примечания

Имя записи устанавливается исключительно в пределах*name* параметр. Имя файла, указанное в*fileInfo* параметр не влияет на имя записи.

*fileInfo* может относиться кDirectoryInfo если запись является каталогом.

Если файл открывается сразу с помощью*openImmediately*параметр блокируется до тех пор, пока архив не будет удален.

### Примеры

```csharp
FileInfo fi = new FileInfo("data.bin");
using (var archive = new TarArchive())
{
   archive.CreateEntry("data.bin", fi);
   archive.Save(tarFile);
}
```

### Смотрите также

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* пространство имен [Aspose.Zip.Tar](../../tararchive/)
* сборка [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Создать одну запись в архиве.

```csharp
public TarEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| path | String | Путь к сжимаемому файлу. |
| openImmediately | Boolean | Истинно, если открыть файл сразу, в противном случае открыть файл при сохранении архива. |

### Возвращаемое значение

Экземпляр записи Tar.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* нулевой. |
| SecurityException | У вызывающего абонента нет необходимого разрешения на доступ. |
| ArgumentException | *path* пуст, содержит только пробелы или содержит недопустимые символы. - или - Имя файла, как часть*name*, превышает 100 символов. |
| UnauthorizedAccessException | Доступ к файлу*path* отказано. |
| PathTooLongException | Указанный*path* , имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. - или -*name* слишком длинный для tar по стандарту IEEE 1003.1-1998. |
| NotSupportedException | Файл в*path* содержит двоеточие (:) в середине строки. |

### Примечания

Имя записи устанавливается исключительно в пределах*name* параметр. Имя файла, указанное в*path* параметр не влияет на имя записи.

Если файл открывается сразу с помощью*openImmediately*параметр блокируется до тех пор, пока архив не будет удален.

### Примеры

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save(outputTarFile);
}
```

### Смотрите также

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* пространство имен [Aspose.Zip.Tar](../../tararchive/)
* сборка [Aspose.Zip](../../../)


