---
title: "SharArchive.CreateEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод SharArchive. Создаёт единственный элемент в архиве"
type: docs
weight: 40
url: /ru/net/aspose.zip.shar/shararchive/createentry/
---
## CreateEntry(string, FileInfo, bool) {#createentry}

Создаёт одну запись внутри архива.

```csharp
public SharEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| fileInfo | FileInfo | Метаданные файла или папки для сжатия. |
| openImmediately | Boolean | True, если файл открывается сразу, иначе файл открывается при сохранении архива. |

### Возвращаемое значение

Экземпляр элемента Shar.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *name* равен null. |
| ArgumentException | *name* пусто. |
| ArgumentNullException | *fileInfo* равен null. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| InvalidOperationException | Этот архив открыт для извлечения. |

## Примечания

Если файл открыт сразу с параметром *openImmediately*, он будет заблокирован до освобождения архива.

## Примеры

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new SharArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.shar");
}
```

### См. также

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Создаёт одну запись внутри архива.

```csharp
public SharEntry CreateEntry(string name, string sourcePath, bool openImmediately = false)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| sourcePath | String | Путь к файлу, который будет сжат. |
| openImmediately | Boolean | True, если файл открывается сразу, иначе файл открывается при сохранении архива. |

### Возвращаемое значение

Экземпляр элемента Shar.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *sourcePath* равен null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | Путь *sourcePath* пуст, содержит только пробелы или содержит недопустимые символы. - or - Имя файла, как часть *name*, превышает 100 символов. |
| UnauthorizedAccessException | Доступ к файлу *sourcePath* запрещён. |
| PathTooLongException | Указанный *sourcePath*, имя файла или оба превышают системно‑определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. - or - *name* слишком длинное для shar. |
| NotSupportedException | Файл по пути *sourcePath* содержит двоеточие (:) в середине строки. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| InvalidOperationException | Этот архив открыт для извлечения. |

## Примечания

Имя элемента задаётся исключительно параметром *name*. Имя файла, переданное в параметре *sourcePath*, не влияет на имя элемента.

Если файл открыт сразу с параметром *openImmediately*, он будет заблокирован до освобождения архива.

## Примеры

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### См. также

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Создаёт одну запись внутри архива.

```csharp
public SharEntry CreateEntry(string name, Stream source)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| source | Stream | Входной поток для записи. |

### Возвращаемое значение

Экземпляр элемента Shar.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *name* равен null. |
| ArgumentNullException | *source* равен null. |
| ArgumentException | *name* пусто. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| InvalidOperationException | Этот архив открыт для извлечения. |

## Примеры

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.shar");
}
```

### См. также

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


