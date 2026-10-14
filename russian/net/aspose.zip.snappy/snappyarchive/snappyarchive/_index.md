---
title: "SnappyArchive.SnappyArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор SnappyArchive. Инициализирует новый экземпляр класса SnappyArchive, подготовленный для сжатия"
type: docs
weight: 10
url: /ru/net/aspose.zip.snappy/snappyarchive/snappyarchive/
---
## SnappyArchive() {#constructor}

Инициализирует новый экземпляр класса [`SnappyArchive`](../), подготовленный для сжатия.

```csharp
public SnappyArchive()
```

## Примеры

В следующем примере показано, как сжать файл.

```csharp
using (SnappyArchive archive = new SnappyArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.snappy");
}
```

### См. также

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## SnappyArchive(Stream) {#constructor_1}

Инициализирует новый экземпляр класса [`SnappyArchive`](../), подготовленный для распаковки.

```csharp
public SnappyArchive(Stream source)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| source | Stream | Источник архива. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *source* не поддерживает поиск. |
| ArgumentNullException | *source* равен null. |

## Примечания

Этот конструктор не распаковывает. См. метод [`Extract`](../extract/) для распаковки.

### См. также

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## SnappyArchive(string) {#constructor_2}

Инициализирует новый экземпляр класса [`SnappyArchive`](../), подготовленный для распаковки.

```csharp
public SnappyArchive(string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к источнику архива. |

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

## Примечания

Этот конструктор не распаковывает. См. метод [`Extract`](../extract/) для распаковки.

## Примеры

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new SnappyArchive(sourceSnappyFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### См. также

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)


