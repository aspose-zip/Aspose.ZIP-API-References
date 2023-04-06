---
title: ArchiveInstanceInfo.GetArchiveFormatInfo
second_title: Aspose.ZIP для справочника API .NET
description: ArchiveInstanceInfo метод. Получает информацию о формате архива.
type: docs
weight: 50
url: /ru/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveformatinfo/
---
## GetArchiveFormatInfo(string) {#getarchiveformatinfo_1}

Получает информацию о формате архива.

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | Имя файла архива. |

### Возвращаемое значение

Информация о формате архива или null, если формат не был обнаружен.

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

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* пространство имен [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* сборка [Aspose.Zip](../../../)

---

## GetArchiveFormatInfo(Stream) {#getarchiveformatinfo}

Получает информацию о формате архива.

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Поток файла архива. |

### Возвращаемое значение

Информация о формате архива или null, если формат не был обнаружен.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *stream* нулевой. |
| ArgumentException | *stream* не доступен для поиска. |

### Смотрите также

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* пространство имен [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* сборка [Aspose.Zip](../../../)


