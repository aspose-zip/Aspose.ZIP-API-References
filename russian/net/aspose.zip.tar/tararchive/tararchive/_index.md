---
title: TarArchive.TarArchive
second_title: Aspose.ZIP для справочника API .NET
description: TarArchive строитель. Инициализирует новый экземплярTarArchive класс.
type: docs
weight: 10
url: /ru/net/aspose.zip.tar/tararchive/tararchive/
---
## TarArchive() {#constructor}

Инициализирует новый экземпляр[`TarArchive`](../) класс.

```csharp
public TarArchive()
```

### Примеры

В следующем примере показано, как сжать файл.

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.tar");
}
```

### Смотрите также

* class [TarArchive](../)
* пространство имен [Aspose.Zip.Tar](../../tararchive/)
* сборка [Aspose.Zip](../../../)

---

## TarArchive(Stream) {#constructor_1}

Инициализирует новый экземпляр[`Archive`](../../../aspose.zip/archive/) список записей классов и композиций можно извлечь из архива.

```csharp
public TarArchive(Stream sourceStream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. Он должен быть доступен для поиска. |

### Исключения

| исключение | условие |
| --- | --- |
| InvalidDataException | *sourceStream* не доступен для поиска. |

### Примечания

Этот конструктор не распаковывает никакую запись. Видеть[`Open`](../../tarentry/open/)способ распаковки.

### Примеры

В следующем примере показано, как извлечь все записи в каталог.

```csharp
using (var archive = new TarArchive(File.OpenRead("archive.tar")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Смотрите также

* class [TarArchive](../)
* пространство имен [Aspose.Zip.Tar](../../tararchive/)
* сборка [Aspose.Zip](../../../)

---

## TarArchive(string) {#constructor_2}

Инициализирует новый экземпляр[`TarArchive`](../) список записей классов и композиций можно извлечь из архива.

```csharp
public TarArchive(string path)
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

Этот конструктор не распаковывает никакую запись. Видеть[`Open`](../../tarentry/open/)способ распаковки.

### Примеры

В следующем примере показано, как извлечь все записи в каталог.

```csharp
using (var archive = new TarArchive("archive.tar")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Смотрите также

* class [TarArchive](../)
* пространство имен [Aspose.Zip.Tar](../../tararchive/)
* сборка [Aspose.Zip](../../../)


