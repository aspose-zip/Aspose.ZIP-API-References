---
title: CabArchive.CabArchive
second_title: Aspose.ZIP для справочника API .NET
description: CabArchive строитель. Инициализирует новый экземплярCabArchive список записей классов и композиций можно извлечь из архива.
type: docs
weight: 10
url: /ru/net/aspose.zip.cab/cabarchive/cabarchive/
---
## CabArchive(Stream) {#constructor}

Инициализирует новый экземпляр[`CabArchive`](../) список записей классов и композиций можно извлечь из архива.

```csharp
public CabArchive(Stream sourceStream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. Он должен быть доступен для поиска. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *sourceStream* нулевой. |
| ArgumentException | *sourceStream* не доступен для поиска. |
| InvalidDataException | *sourceStream* недействителен каб-архив. |

### Примечания

Этот конструктор не распаковывает никакую запись. Видеть[`Open`](../../cabentry/open/)способ распаковки.

### Примеры

В следующем примере показано, как извлечь все записи в каталог.

```csharp
using (var archive = new CabArchive(File.OpenRead("archive.cab")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Смотрите также

* class [CabArchive](../)
* пространство имен [Aspose.Zip.Cab](../../cabarchive/)
* сборка [Aspose.Zip](../../../)

---

## CabArchive(string) {#constructor_1}

Инициализирует новый экземпляр[`CabArchive`](../) список записей классов и композиций можно извлечь из архива.

```csharp
public CabArchive(string path)
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

Этот конструктор не распаковывает никакую запись. Видеть[`Open`](../../cabentry/open/)способ распаковки.

### Примеры

В следующем примере показано, как извлечь все записи в каталог.

```csharp
using (var archive = new CabArchive("archive.cab")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Смотрите также

* class [CabArchive](../)
* пространство имен [Aspose.Zip.Cab](../../cabarchive/)
* сборка [Aspose.Zip](../../../)


