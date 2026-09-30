---
title: "CpioArchive.CpioArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор CpioArchive. Инициализирует новый экземпляр класса CpioArchive."
type: docs
weight: 10
url: /ru/net/aspose.zip.cpio/cpioarchive/cpioarchive/
---
## CpioArchive() {#constructor}

Инициализирует новый экземпляр класса [`CpioArchive`](../).

```csharp
public CpioArchive()
```

## Примеры

В следующем примере показано, как сжать файл.

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cpio");
}
```

### См. также

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## CpioArchive(Stream) {#constructor_1}

Инициализирует новый экземпляр класса [`CpioArchive`](../) и формирует список записей, который может быть извлечён из архива.

```csharp
public CpioArchive(Stream sourceStream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. Должен поддерживать поиск. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *sourceStream* имеет значение null. |
| ArgumentException | *sourceStream* не поддерживает перемещение. |
| InvalidDataException | *sourceStream* не является действительным архивом cpio. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до того, как все байты заголовка или имени были прочитаны. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |
| IOException | Произошла ошибка ввода/вывода. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`Open`](../../cpioentry/open/) для распаковки.

## Примеры

В следующем примере показано, как извлечь все записи в каталог.

```csharp
using (var archive = new CpioArchive(File.OpenRead("archive.cpio")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### См. также

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## CpioArchive(string) {#constructor_2}

Инициализирует новый экземпляр класса [`CpioArchive`](../) и формирует список записей, который может быть извлечён из архива.

```csharp
public CpioArchive(string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу архива. |

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
| EndOfStreamException | Выбрасывается, когда конец потока достигается до того, как все байты заголовка или имени были прочитаны. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |
| InvalidDataException | Выбрасывается, когда данные недействительны или повреждены. |

## Примечания

Этот конструктор не распаковывает ни одну запись. См. метод [`Open`](../../cpioentry/open/) для распаковки.

## Примеры

В следующем примере показано, как извлечь все записи в каталог.

```csharp
using (var archive = new CpioArchive("archive.cpio")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### См. также

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


