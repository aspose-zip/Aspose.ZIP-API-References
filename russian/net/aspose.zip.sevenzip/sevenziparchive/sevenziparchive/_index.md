---
title: "SevenZipArchive.SevenZipArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор SevenZipArchive. Инициализирует новый экземпляр класса SevenZipArchive с необязательными параметрами для его записей."
type: docs
weight: 10
url: /ru/net/aspose.zip.sevenzip/sevenziparchive/sevenziparchive/
---
## SevenZipArchive(SevenZipEntrySettings) {#constructor}

Инициализирует новый экземпляр класса [`SevenZipArchive`](../) с необязательными параметрами для его записей.

```csharp
public SevenZipArchive(SevenZipEntrySettings newEntrySettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| newEntrySettings | SevenZipEntrySettings | Параметры сжатия и шифрования, используемые для недавно добавленных элементов [`SevenZipArchiveEntry`](../../sevenziparchiveentry/). Если не указано, будет использовано сжатие LZMA без шифрования. |

## Примеры

Следующий пример показывает, как сжать один файл с настройками по умолчанию: сжатие LZMA без шифрования.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### См. также

* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive(Stream, string) {#constructor_2}

Инициализирует новый экземпляр класса [`SevenZipArchive`](../) и формирует список записей, который можно извлечь из архива.

```csharp
public SevenZipArchive(Stream sourceStream, string password = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. |
| password | String | Необязательный пароль для расшифровки. Если имена файлов зашифрованы, он должен быть указан. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *sourceStream* не поддерживает перемещение. |
| ArgumentNullException | *sourceStream* имеет значение null. |
| NotImplementedException | В архиве содержится более одного кодера. Сейчас поддерживается только сжатие LZMA. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`ExtractToDirectory`](../extracttodirectory/) для распаковки.

## Примеры

```csharp
using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z")))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### См. также

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive(string, string) {#constructor_4}

Инициализирует новый экземпляр класса [`SevenZipArchive`](../) и формирует список записей, который можно извлечь из архива.

```csharp
public SevenZipArchive(string path, string password = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Полный или относительный путь к файлу архива. |
| password | String | Необязательный пароль для расшифровки. Если имена файлов зашифрованы, он должен быть указан. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* имеет значение null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | *path* пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *path* запрещён. |
| PathTooLongException | Указанный *path*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл по адресу *path* содержит двоеточие (:) в середине строки. |
| FileNotFoundException | Файл не найден. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| IOException | Файл уже открыт. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`ExtractToDirectory`](../extracttodirectory/) для распаковки.

## Примеры

```csharp
using (SevenZipArchive archive = new SevenZipArchive("archive.7z"))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### См. также

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive(Stream, SevenZipLoadOptions) {#constructor_1}

Инициализирует новый экземпляр класса [`SevenZipArchive`](../) и формирует список записей, который можно извлечь из архива.

```csharp
public SevenZipArchive(Stream sourceStream, SevenZipLoadOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. |
| параметры | SevenZipLoadOptions | Параметры загрузки существующего архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *sourceStream* не поддерживает перемещение. |
| ArgumentNullException | *sourceStream* имеет значение null. |
| NotImplementedException | В архиве содержится более одного кодера. Сейчас поддерживается только сжатие LZMA. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |
| IOException | Произошла ошибка ввода/вывода. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`ExtractToDirectory`](../extracttodirectory/) для распаковки.

## Примеры

Извлечь зашифрованный архив. Позволяет работать до 60 секунд, после этого периода отменить.

```csharp
using(CancellationTokenSource cts = new CancellationTokenSource())
{
    SevenZipLoadOptions options = new SevenZipLoadOptions(){ DecryptionPassword = "Top$ecr3t", CancellationToken = cts.Token }
    cts.CancelAfter(TimeSpan.FromSeconds(60));
    using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z"), options))
    {
        archive.ExtractToDirectory("C:\\extracted");
    }
}
```

### См. также

* class [SevenZipLoadOptions](../../sevenziploadoptions/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive(string, SevenZipLoadOptions) {#constructor_3}

Инициализирует новый экземпляр класса [`SevenZipArchive`](../) и формирует список записей, который можно извлечь из архива.

```csharp
public SevenZipArchive(string path, SevenZipLoadOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Полный или относительный путь к файлу архива. |
| параметры | SevenZipLoadOptions | Параметры загрузки существующего архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* имеет значение null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | *path* пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *path* запрещён. |
| PathTooLongException | Указанный *path*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл по адресу *path* содержит двоеточие (:) в середине строки. |
| FileNotFoundException | Файл не найден. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| IOException | Файл уже открыт. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`ExtractToDirectory`](../extracttodirectory/) для распаковки.

## Примеры

Извлечь зашифрованный архив. Позволяет работать до 60 секунд, после этого периода отменить.

```csharp
using(CancellationTokenSource cts = new CancellationTokenSource())
{
    SevenZipLoadOptions options = new SevenZipLoadOptions(){ DecryptionPassword = "Top$ecr3t", CancellationToken = cts.Token }
    cts.CancelAfter(TimeSpan.FromSeconds(60));
    using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z"), options))
    {
        archive.ExtractToDirectory("C:\\extracted");
    }
}
```

### См. также

* class [SevenZipLoadOptions](../../sevenziploadoptions/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive(string[], string) {#constructor_5}

Инициализирует новый экземпляр класса [`SevenZipArchive`](../) из многотомного 7z‑архива и формирует список записей, которые можно извлечь из архива.

```csharp
public SevenZipArchive(string[] parts, string password = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| parts | String[] | Пути к каждому сегменту многотомного 7z‑архива в порядке следования |
| password | String | Необязательный пароль для расшифровки. Если имена файлов зашифрованы, он должен быть указан. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *parts* равно null. |
| ArgumentException | *parts* не содержит записей. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | Путь к файлу пустой, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу запрещён. |
| PathTooLongException | Указанный путь к части, имя файла или оба превышают системно‑определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл по пути содержит двоеточие (:) в середине строки. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| FileNotFoundException | Файл не найден. |
| IOException | Файл уже открыт. |

## Примеры

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new string[] { "multi.7z.001", "multi.7z.002", "multi.7z.003" }))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### См. также

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


