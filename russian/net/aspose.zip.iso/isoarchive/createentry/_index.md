---
title: "IsoArchive.CreateEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод IsoArchive. Добавляет файл в образ ISO"
type: docs
weight: 40
url: /ru/net/aspose.zip.iso/isoarchive/createentry/
---
## CreateEntry(string, string) {#createentry_2}

Добавляет файл в ISO‑образ.

```csharp
public IsoEntry CreateEntry(string name, string filePath)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Путь к файлу в ISO. |
| filePath | String | Путь к файлу. |

### Возвращаемое значение

Элемент ISO составлен.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | Значение *filePath* равно null. |
| ArgumentException | Значение *filePath* пусто, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *filePath* запрещён. |
| PathTooLongException | Указанный *filePath* превышает системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл по пути *filePath* содержит двоеточие (:) в середине строки. |
| IOException | Во время открытия файла произошла ошибка ввода/вывода. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| DirectoryNotFoundException | Указанный путь недействителен (например, он находится на не смонтированном диске). |
| FileNotFoundException | Файл, указанный в *filePath*, не найден. |
| InvalidOperationException | Архив не находится в режиме редактирования. |

### См. также

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Добавляет файл в ISO‑образ.

```csharp
public IsoEntry CreateEntry(string name, Stream source)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Путь к файлу в ISO. |
| source | Stream | Поток, содержащий данные файла. |

### Возвращаемое значение

Элемент ISO составлен.

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| ArgumentNullException | Выбрасывается, когда *name* или *source* равны null. |
| InvalidOperationException | Архив не находится в режиме редактирования. |

### См. также

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string) {#createentry}

Добавляет файл в ISO‑образ.

```csharp
public IsoEntry CreateEntry(string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Путь к каталогу в ISO. |

### Возвращаемое значение

Элемент ISO составлен.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | `name` имеет значение null или пустой. |
| InvalidOperationException | Архив открыт для извлечения. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

### См. также

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


