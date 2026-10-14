---
title: "IsoArchive.IsoArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор IsoArchive. Инициализирует новый экземпляр класса IsoArchive и создаёт пустой ISO‑архив для добавления новых файлов и каталогов."
type: docs
weight: 10
url: /ru/net/aspose.zip.iso/isoarchive/isoarchive/
---
## IsoArchive() {#constructor}

Инициализирует новый экземпляр класса [`IsoArchive`](../) и создаёт пустой ISO‑архив для добавления новых файлов и каталогов.

```csharp
public IsoArchive()
```

## Примеры

Следующий пример показывает, как создать новый пустой ISO‑архив и добавить в него файлы:

```csharp
// Создать новый пустой ISO‑архив
using(IsoArchive isoArchive = new IsoArchive())
{
    // Добавить файлы в ISO‑архив
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // Сохранить ISO‑архив в файл
    isoArchive.Save("new_archive.iso");
}
```

### См. также

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(Stream, IsoLoadOptions) {#constructor_1}

Инициализирует новый экземпляр класса [`IsoArchive`](../) и формирует список записей, которые можно извлечь из архива.

```csharp
public IsoArchive(Stream sourceStream, IsoLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. Должен поддерживать поиск. |
| loadOptions | IsoLoadOptions | Параметры загрузки архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *sourceStream* имеет значение null. |
| ArgumentException | *sourceStream* не поддерживает перемещение. |
| InvalidDataException | *sourceStream* не является действительным ISO-архивом. |
| ObjectDisposedException | Выбрасывается, если исходный поток был освобождён. |
| EndOfStreamException | Выбрасывается, когда конец потока достигается неожиданно. |
| IOException | Произошла ошибка ввода/вывода. |
| NotSupportedException | Поток не поддерживает чтение. |

## Примечания

Этот конструктор не распаковывает ни одну запись.

## Примеры

В следующем примере показано, как извлечь все записи в каталог.

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### См. также

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(string, IsoLoadOptions) {#constructor_2}

Инициализирует новый экземпляр класса [`IsoArchive`](../) и формирует список записей, которые можно извлечь из архива.

```csharp
public IsoArchive(string path, IsoLoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу архива. |
| loadOptions | IsoLoadOptions | Параметры загрузки архива. |

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
| EndOfStreamException | Файл слишком короткий. |
| InvalidDataException | Выбрасывается, когда данные недействительны или повреждены. |

## Примечания

Этот конструктор не распаковывает ни одну запись.

## Примеры

В следующем примере показано, как извлечь все записи в каталог.

```csharp
using (var archive = new IsoArchive("archive.iso")) 
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### См. также

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


