---
title: XarArchive.XarArchive
second_title: Aspose.ZIP для справочника API .NET
description: XarArchive строитель. Инициализирует новый экземплярXarArchive список записей классов и композиций можно извлечь из архива.
type: docs
weight: 10
url: /ru/net/aspose.zip.xar/xararchive/xararchive/
---
## XarArchive(Stream) {#constructor}

Инициализирует новый экземпляр[`XarArchive`](../) список записей классов и композиций можно извлечь из архива.

```csharp
public XarArchive(Stream sourceStream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. Он должен быть доступен для поиска. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *sourceStream* нулевой. |
| ArgumentException | *sourceStream* не доступен для поиска. |
| InvalidDataException | *sourceStream* недопустимый xar-архив. |

### Примечания

Этот конструктор не распаковывает никакую запись. Видеть[`Open`](../../xarfileentry/open/)способ распаковки.

### Примеры

В следующем примере показано, как извлечь все записи в каталог.

```csharp
using (var archive = new XarArchive(File.OpenRead("archive.xar")))
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Смотрите также

* class [XarArchive](../)
* пространство имен [Aspose.Zip.Xar](../../xararchive/)
* сборка [Aspose.Zip](../../../)

---

## XarArchive(string) {#constructor_1}

Инициализирует новый экземпляр[`XarArchive`](../) список записей классов и композиций можно извлечь из архива.

```csharp
public XarArchive(string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу архива. |

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

Этот конструктор не распаковывает никакую запись. Видеть[`Open`](../../xarfileentry/open/)способ распаковки.

### Примеры

В следующем примере показано, как извлечь все записи в каталог.

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Смотрите также

* class [XarArchive](../)
* пространство имен [Aspose.Zip.Xar](../../xararchive/)
* сборка [Aspose.Zip](../../../)


