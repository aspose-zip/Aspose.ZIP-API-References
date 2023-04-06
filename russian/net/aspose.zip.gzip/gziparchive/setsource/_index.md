---
title: GzipArchive.SetSource
second_title: Aspose.ZIP для справочника API .NET
description: GzipArchive метод. Задает сжатие содержимого внутри архива.
type: docs
weight: 70
url: /ru/net/aspose.zip.gzip/gziparchive/setsource/
---
## SetSource(Stream) {#setsource_2}

Задает сжатие содержимого внутри архива.

```csharp
public void SetSource(Stream source)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| source | Stream | Входной поток для архива. |

### Примеры

```csharp
using (var archive = new GzipArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.gz");
}
```

### Смотрите также

* class [GzipArchive](../)
* пространство имен [Aspose.Zip.Gzip](../../gziparchive/)
* сборка [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

Задает сжатие содержимого внутри архива.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileInfo | FileInfo | Ссылка на файл, который нужно сжать. |

### Примеры

Откройте архив из потока и распакуйте его в`ПамятьПоток`

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.gz");
}
```

### Смотрите также

* class [GzipArchive](../)
* пространство имен [Aspose.Zip.Gzip](../../gziparchive/)
* сборка [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

Задает сжатие содержимого внутри архива.

```csharp
public void SetSource(string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к сжимаемому файлу. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* нулевой. |
| SecurityException | У вызывающего абонента нет необходимого разрешения на доступ. |
| ArgumentException | *path* пуст, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу*path* отказано. |
| PathTooLongException | Указанный*path*, имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. |
| NotSupportedException | Файл в*path* содержит двоеточие (:) в середине строки. |

### Примеры

Откройте архив из файла по пути и извлеките его в`ПамятьПоток`

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### Смотрите также

* class [GzipArchive](../)
* пространство имен [Aspose.Zip.Gzip](../../gziparchive/)
* сборка [Aspose.Zip](../../../)

---

## SetSource(TarArchive) {#setsource}

Задает сжатие содержимого внутри архива.

```csharp
public void SetSource(TarArchive tarArchive)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| tarArchive | TarArchive | Архив Tar для сжатия. |

### Примечания

Используйте этот метод для создания совместного архива tar.gz.

### Примеры

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var gzippedArchive = new GzipArchive())
    {
           gzippedArchive.SetSource(tarArchive);
           gzippedArchive.Save("archive.tar.gz");
    }
}
```

### Смотрите также

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* class [GzipArchive](../)
* пространство имен [Aspose.Zip.Gzip](../../gziparchive/)
* сборка [Aspose.Zip](../../../)


