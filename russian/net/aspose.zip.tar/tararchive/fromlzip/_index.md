---
title: "TarArchive.FromLZip"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод TarArchive. Извлекает предоставленный lzip‑архив и создает TarArchive из извлечённых данных."
type: docs
weight: 40
url: /ru/net/aspose.zip.tar/tararchive/fromlzip/
---
## FromLZip(Stream) {#fromlzip}

Извлекает предоставленный архив lzip и создает [`TarArchive`](../) из извлечённых данных.

Важно: архив lzip полностью извлекается в этом методе, его содержимое хранится внутри. Будьте внимательны к потреблению памяти.

```csharp
public static TarArchive FromLZip(Stream source)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| source | Stream | Источник архива. |

### Возвращаемое значение

Экземпляр [`TarArchive`](../)

### Исключения

| исключение | условие |
| --- | --- |
| InvalidDataException | Архив повреждён. |
| ArgumentException | *source* не поддерживает поиск. |
| ArgumentNullException | *source* равен null. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |
| IOException | Произошла ошибка ввода/вывода. |
| InvalidOperationException | Заголовки архива и служебная информация не были прочитаны. |

## Примечания

Поток извлечения lzip не поддерживает перемещение, что обусловлено природой алгоритма сжатия. Архив Tar предоставляет возможность извлекать произвольные записи, поэтому он должен работать с перемещаемым потоком в основе.

### См. также

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZip(string) {#fromlzip_1}

Извлекает предоставленный архив lzip и создает [`TarArchive`](../) из извлечённых данных.

Важно: архив lzip полностью извлекается в этом методе, его содержимое хранится внутри. Будьте внимательны к потреблению памяти.

```csharp
public static TarArchive FromLZip(string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу архива. |

### Возвращаемое значение

Экземпляр [`TarArchive`](../)

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* имеет значение null. |
| ArgumentException | *path* пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *path* запрещён. |
| PathTooLongException | Указанный *path*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл по пути *path* имеет недопустимый формат. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| FileNotFoundException | Файл не найден. |
| InvalidDataException | Архив повреждён. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| IOException | Произошла ошибка ввода/вывода. |
| InvalidOperationException | Заголовки архива и служебная информация не были прочитаны. |

## Примечания

Поток извлечения lzip не поддерживает перемещение, что обусловлено природой алгоритма сжатия. Архив Tar предоставляет возможность извлекать произвольные записи, поэтому он должен работать с перемещаемым потоком в основе.

### См. также

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


