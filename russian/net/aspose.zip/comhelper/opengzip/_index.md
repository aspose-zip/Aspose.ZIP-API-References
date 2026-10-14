---
title: "ComHelper.OpenGzip"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод ComHelper. Позволяет COM‑приложению загрузить gzip‑архив из потока"
type: docs
weight: 30
url: /ru/net/aspose.zip/comhelper/opengzip/
---
## OpenGzip(Stream) {#opengzip}

Позволяет COM‑приложению загрузить архив gzip из потока.

```csharp
public GzipArchive OpenGzip(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Объект .NET‑потока, содержащий архив для загрузки. |

### Возвращаемое значение

Объект [`GzipArchive`](../../../aspose.zip.gzip/gziparchive/), представляющий архив.

### Исключения

| исключение | условие |
| --- | --- |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| ArgumentNullException | Выбрасывается, когда *stream* равен null. |
| InvalidDataException | Выбрасывается, когда данные недействительны или повреждены. |

### См. также

* class [GzipArchive](../../../aspose.zip.gzip/gziparchive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)

---

## OpenGzip(string) {#opengzip_1}

Позволяет COM‑приложению загрузить gzip‑архив из файла.

```csharp
public GzipArchive OpenGzip(string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | Имя файла архива для загрузки. |

### Возвращаемое значение

Объект [`GzipArchive`](../../../aspose.zip.gzip/gziparchive/), представляющий архив.

### Исключения

| исключение | условие |
| --- | --- |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| ArgumentException | Имя файла пустое, содержит только пробелы или содержит недопустимые символы. |
| ArgumentNullException | *fileName* равно `null`. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| FileNotFoundException | Файл не найден. |
| InvalidDataException | Выбрасывается, когда данные недействительны или повреждены. |
| PathTooLongException | Указанный путь, имя файла или их комбинация превышают системно определённую максимальную длину. |
| UnauthorizedAccessException | Доступ к *fileName* запрещён. |

### См. также

* class [GzipArchive](../../../aspose.zip.gzip/gziparchive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)


