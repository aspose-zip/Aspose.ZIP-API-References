---
title: CpioArchive.CpioArchive
second_title: Aspose.ZIP для справочника API .NET
description: CpioArchive строитель. Инициализирует новый экземплярCpioArchive класс.
type: docs
weight: 10
url: /ru/net/aspose.zip.cpio/cpioarchive/cpioarchive/
---
## CpioArchive() {#constructor}

Инициализирует новый экземпляр[`CpioArchive`](../) класс.

```csharp
public CpioArchive()
```

### Примеры

В следующем примере показано, как сжать файл.

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cpio");
}
```

### Смотрите также

* class [CpioArchive](../)
* пространство имен [Aspose.Zip.Cpio](../../cpioarchive/)
* сборка [Aspose.Zip](../../../)

---

## CpioArchive(Stream) {#constructor_1}

Инициализирует новый экземпляр[`CpioArchive`](../) список записей классов и композиций можно извлечь из архива.

```csharp
public CpioArchive(Stream sourceStream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. Он должен быть доступен для поиска. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *sourceStream* нулевой. |
| ArgumentException | *sourceStream* не доступен для поиска. |
| InvalidDataException | *sourceStream* недействительный архив cpio. |

### Примечания

Этот конструктор не распаковывает никакую запись. Видеть[`Open`](../../cpioentry/open/)способ распаковки.

### Примеры

В следующем примере показано, как извлечь все записи в каталог.

```csharp
using (var archive = new CpioArchive(File.OpenRead("archive.cpio")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Смотрите также

* class [CpioArchive](../)
* пространство имен [Aspose.Zip.Cpio](../../cpioarchive/)
* сборка [Aspose.Zip](../../../)

---

## CpioArchive(string) {#constructor_2}

Инициализирует новый экземпляр[`CpioArchive`](../) список записей классов и композиций можно извлечь из архива.

```csharp
public CpioArchive(string path)
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

Этот конструктор не распаковывает никакую запись. Видеть[`Open`](../../cpioentry/open/)способ распаковки.

### Примеры

В следующем примере показано, как извлечь все записи в каталог.

```csharp
using (var archive = new CpioArchive("archive.cpio")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Смотрите также

* class [CpioArchive](../)
* пространство имен [Aspose.Zip.Cpio](../../cpioarchive/)
* сборка [Aspose.Zip](../../../)


