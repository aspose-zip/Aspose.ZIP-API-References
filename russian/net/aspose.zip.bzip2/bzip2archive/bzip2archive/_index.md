---
title: "Bzip2Archive.Bzip2Archive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор Bzip2Archive. Инициализирует новый экземпляр класса Bzip2Archive, подготовленный для сжатия."
type: docs
weight: 10
url: /ru/net/aspose.zip.bzip2/bzip2archive/bzip2archive/
---
## Bzip2Archive() {#constructor}

Инициализирует новый экземпляр класса [`Bzip2Archive`](../), подготовленный для сжатия.

```csharp
public Bzip2Archive()
```

## Примеры

В следующем примере показано, как сжать файл.

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### См. также

* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)

---

## Bzip2Archive(Stream, Bzip2LoadOptions) {#constructor_1}

Инициализирует новый экземпляр класса [`Bzip2Archive`](../), подготовленный для распаковки.

```csharp
public Bzip2Archive(Stream sourceStream, Bzip2LoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | Stream | Источник архива. |
| loadOptions | Bzip2LoadOptions | Параметры загрузки архива. |

### Исключения

| исключение | условие |
| --- | --- |
| EndOfStreamException | Преждевременный конец потока. |
| InvalidDataException | Неправильные байты сигнатуры. |
| IOException | Произошла ошибка ввода/вывода. |
| ArgumentNullException | *sourceStream* имеет значение null. |

## Примечания

Этот конструктор не выполняет распаковку. См. метод [`Open`](../open/) для распаковки.

## Примеры

Откройте архив из потока и извлеките его в `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive(File.OpenRead("archive.bz2")))
  archive.Open().CopyTo(ms);
```

### См. также

* class [Bzip2LoadOptions](../../bzip2loadoptions/)
* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)

---

## Bzip2Archive(string, Bzip2LoadOptions) {#constructor_2}

Инициализирует новый экземпляр класса [`Bzip2Archive`](../), подготовленный для распаковки.

```csharp
public Bzip2Archive(string path, Bzip2LoadOptions loadOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу архива. |
| loadOptions | Bzip2LoadOptions | Параметры загрузки архива. |

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
| EndOfStreamException | Преждевременный конец потока. |
| InvalidDataException | Неправильные байты сигнатуры. |

## Примечания

Этот конструктор не выполняет распаковку. См. метод [`Open`](../open/) для распаковки.

## Примеры

Откройте архив из файла по пути и извлеките его в `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
  archive.Open().CopyTo(ms);
```

### См. также

* class [Bzip2LoadOptions](../../bzip2loadoptions/)
* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)


