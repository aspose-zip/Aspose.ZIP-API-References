---
title: RarArchive.RarArchive
second_title: Aspose.ZIP для справочника API .NET
description: RarArchive строитель. Инициализирует новый экземплярRarArchive список записей классов и композиций можно извлечь из архива.
type: docs
weight: 10
url: /ru/net/aspose.zip.rar/rararchive/rararchive/
---
## RarArchive(string, RarArchiveLoadOptions) {#constructor_1}

Инициализирует новый экземпляр[`RarArchive`](../) список записей классов и композиций можно извлечь из архива.

```csharp
public RarArchive(string path, RarArchiveLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Полный или относительный путь к файлу архива. |
| loadOptions | RarArchiveLoadOptions | Опции для загрузки существующего архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* нулевой. |
| SecurityException | У вызывающего абонента нет необходимого разрешения на доступ. |
| ArgumentException | *path* пуст, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу*path* отказано. |
| PathTooLongException | Указанный*path*, имя файла или оба превышают максимальную длину, определенную системой. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. |
| NotSupportedException | Файл в*path* содержит двоеточие (:) в середине строки. |

### Примечания

Этот конструктор не распаковывает никакие записи. Видеть[`Open`](../../rararchiveentry/open/) метод распаковки.

### Примеры

В следующем примере извлекается архив, а затем распаковывается первая запись в`ПамятьПоток`.

```csharp
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive("data.rar"))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Смотрите также

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* пространство имен [Aspose.Zip.Rar](../../rararchive/)
* сборка [Aspose.Zip](../../../)

---

## RarArchive(Stream, RarArchiveLoadOptions) {#constructor}

Инициализирует новый экземпляр[`RarArchive`](../) список записей классов и композиций можно извлечь из архива.

```csharp
public RarArchive(Stream sourceStream, RarArchiveLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. |
| loadOptions | RarArchiveLoadOptions | Опции для загрузки существующего архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *sourceStream* не доступен для поиска. |
| InvalidDataException | Неправильная подпись для архива. - или - Файл не является архивом RAR. |
| InvalidOperationException |  |

### Примечания

Этот конструктор не распаковывает никакие записи. Видеть[`Open`](../../rararchiveentry/open/) метод распаковки.

### Примеры

В следующем примере расшифровывается и распаковывается первая запись в`ПамятьПоток`.

```csharp
var fs = File.OpenRead("encrypted.rar");
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive(fs, new RarArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Смотрите также

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* пространство имен [Aspose.Zip.Rar](../../rararchive/)
* сборка [Aspose.Zip](../../../)


