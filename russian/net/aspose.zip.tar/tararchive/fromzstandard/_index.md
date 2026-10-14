---
title: "TarArchive.FromZstandard"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод TarArchive. Извлекает предоставленный Zstandard‑архив и создает TarArchive из извлечённых данных."
type: docs
weight: 80
url: /ru/net/aspose.zip.tar/tararchive/fromzstandard/
---
## FromZstandard(Stream) {#fromzstandard}

Извлекает предоставленный Zstandard‑архив и создает [`TarArchive`](../) из извлечённых данных.

Важно: Zstandard‑архив полностью извлекается в этом методе, его содержимое хранится во внутренней памяти. Будьте внимательны к потреблению памяти.

```csharp
public static TarArchive FromZstandard(Stream source)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| source | Stream | Источник архива. |

### Возвращаемое значение

Экземпляр [`TarArchive`](../)

### Исключения

| исключение | условие |
| --- | --- |
| IOException | Поток Zstandard повреждён или нечитаем. |
| InvalidDataException | Данные повреждены. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |

### См. также

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromZstandard(string) {#fromzstandard_1}

Извлекает предоставленный Zstandard‑архив и создает [`TarArchive`](../) из извлечённых данных.

Важно: Zstandard‑архив полностью извлекается в этом методе, его содержимое хранится во внутренней памяти. Будьте внимательны к потреблению памяти.

```csharp
public static TarArchive FromZstandard(string path)
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
| IOException | Поток Zstandard повреждён или нечитаем. |
| InvalidDataException | Данные повреждены. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |

### См. также

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


