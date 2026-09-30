---
title: "TarArchive.FromLZ4"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод TarArchive. Извлекает предоставленный архив LZ4 и создает TarArchive из извлечённых данных"
type: docs
weight: 30
url: /ru/net/aspose.zip.tar/tararchive/fromlz4/
---
## FromLZ4(string) {#fromlz4_1}

Извлекает предоставленный архив LZ4 и создает [`TarArchive`](../) из извлечённых данных.

Важно: архив LZ4 полностью извлекается в этом методе, его содержимое хранится внутри. Будьте внимательны к потреблению памяти.

```csharp
public static TarArchive FromLZ4(string path)
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
| SecurityException | Вызвавший процесс не имеет необходимого разрешения для доступа. |
| ArgumentException | *path* пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *path* запрещён. |
| PathTooLongException | Указанный *path*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл по пути *path* имеет недопустимый формат. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| FileNotFoundException | Файл не найден. |
| EndOfStreamException | Файл слишком короткий. |
| InvalidDataException | Файл имеет неправильную сигнатуру. |
| IOException | Во время открытия файла произошла ошибка ввода/вывода. |
| InvalidOperationException | Архив подготовлен для компоновки. |

## Примечания

Поток извлечения LZ4 не поддерживает перемещение, что обусловлено природой алгоритма сжатия. Архив Tar предоставляет возможность извлекать произвольные записи, поэтому он должен работать с перемещаемым потоком в основе.

### См. также

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZ4(Stream) {#fromlz4}

Извлекает предоставленный архив LZ4 и создает [`TarArchive`](../) из извлечённых данных.

Важно: архив LZ4 полностью извлекается в этом методе, его содержимое хранится внутри. Будьте внимательны к потреблению памяти.

```csharp
public static TarArchive FromLZ4(Stream source)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| source | Stream | Источник архива. |

### Возвращаемое значение

Экземпляр [`TarArchive`](../)

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | Не удалось прочитать из *source* |
| ArgumentNullException | *source* равен null. |
| EndOfStreamException | *source* слишком короткий. |
| InvalidDataException | *source* имеет неправильную сигнатуру. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |

## Примечания

Поток извлечения LZ4 не поддерживает перемещение, что обусловлено природой алгоритма сжатия. Архив Tar предоставляет возможность извлекать произвольные записи, поэтому он должен работать с перемещаемым потоком в основе.

### См. также

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


