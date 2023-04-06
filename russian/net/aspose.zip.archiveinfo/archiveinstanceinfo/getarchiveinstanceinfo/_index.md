---
title: ArchiveInstanceInfo.GetArchiveInstanceInfo
second_title: Aspose.ZIP для справочника API .NET
description: ArchiveInstanceInfo метод. Получает информацию об экземпляре архива.
type: docs
weight: 10
url: /ru/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveinstanceinfo/
---
## GetArchiveInstanceInfo(string) {#getarchiveinstanceinfo_1}

Получает информацию об экземпляре архива.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | Имя файла архива. |

### Возвращаемое значение

Информация об экземпляре архива или null, если формат не был обнаружен.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *fileName* нулевой. |
| SecurityException | У вызывающего абонента нет необходимого разрешения на доступ. |
| ArgumentException | *fileName* пуст, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу*fileName* отказано. |
| PathTooLongException | Указанный*fileName* превышает заданную системой максимальную длину. Например, на платформах Windows пути должны содержать менее 248 символов, а имена файлов — менее 260 символов. |
| NotSupportedException | Файл в*fileName* содержит двоеточие (:) в середине строки. |
| IOException | Ошибка ввода-вывода при открытии файла. |

### Смотрите также

* class [ArchiveInstanceInfo](../)
* пространство имен [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* сборка [Aspose.Zip](../../../)

---

## GetArchiveInstanceInfo(Stream) {#getarchiveinstanceinfo}

Получает информацию об экземпляре архива.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Поток файла архива. |

### Возвращаемое значение

Информация об экземпляре архива или null, если формат не был обнаружен.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *stream* нулевой. |
| ArgumentException | *stream* не доступен для поиска. |

### Смотрите также

* class [ArchiveInstanceInfo](../)
* пространство имен [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* сборка [Aspose.Zip](../../../)


