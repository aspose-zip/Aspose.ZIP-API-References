---
title: "AppleArchive.CreateEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод AppleArchive. Создаёт одну запись в архиве"
type: docs
weight: 60
url: /ru/net/aspose.zip.apple/applearchive/createentry/
---
## CreateEntry(string, string, bool) {#createentry_2}

Создает одну запись в архиве.

```csharp
public AppleArchiveEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| path | String | Путь к файлу для сжатия. |
| openImmediately | Boolean | True, если файл открывается сразу, иначе файл открывается при сохранении архива. |

### Возвращаемое значение

Экземпляр записи Apple Archive.

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Архив был освобождён. |
| ArgumentException | *name* пусто. |
| ArgumentNullException | *path* равно `null`. |

### См. также

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Создает одну запись в архиве.

```csharp
public AppleArchiveEntry CreateEntry(string name, Stream source)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| source | Stream | Входной поток для записи. |

### Возвращаемое значение

Экземпляр записи Apple Archive.

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Архив был освобождён. |
| ArgumentException | *name* пусто. |
| ArgumentNullException | *source* равен `null`. |

### См. также

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Создает одну запись в архиве.

```csharp
public AppleArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя записи. |
| fileInfo | FileInfo | Метаданные файла для сжатия. |
| openImmediately | Boolean | True, если файл открывается сразу, иначе файл открывается при сохранении архива. |

### Возвращаемое значение

Экземпляр записи Apple Archive.

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Архив был освобождён. |
| ArgumentException | *name* пусто. |
| ArgumentNullException | *fileInfo* равен `null`. |

### См. также

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


