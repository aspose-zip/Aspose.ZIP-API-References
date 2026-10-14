---
title: "ArchiveInstanceInfo.GetArchiveInstanceInfo"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод ArchiveInstanceInfo. Возвращает информацию об экземпляре архива."
type: docs
weight: 10
url: /ru/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveinstanceinfo/
---
## GetArchiveInstanceInfo(string) {#getarchiveinstanceinfo_1}

Возвращает информацию о экземпляре архива.

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
| ArgumentNullException | *fileName* равно null. |
| SecurityException | Вызвавший не имеет необходимого разрешения для доступа. |
| ArgumentException | Файл *fileName* пуст, содержит только пробелы или содержит недопустимые символы. |
| UnauthorizedAccessException | Доступ к файлу *fileName* запрещён. |
| PathTooLongException | Указанный *fileName* превышает системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| NotSupportedException | Файл по пути *fileName* содержит двоеточие (:) в середине строки. |
| IOException | Во время открытия файла произошла ошибка ввода/вывода. |
| DirectoryNotFoundException | Указанный путь недействителен (например, он находится на не смонтированном диске). |
| FileNotFoundException | Указанный файл не найден. |

### См. также

* class [ArchiveInstanceInfo](../)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* assembly [Aspose.Zip](../../../)

---

## GetArchiveInstanceInfo(Stream) {#getarchiveinstanceinfo}

Возвращает информацию о экземпляре архива.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Поток архивного файла. |

### Возвращаемое значение

Информация об экземпляре архива или null, если формат не был обнаружен.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *stream* равно null. |
| ArgumentException | *stream* не поддерживает поиск. |

### См. также

* class [ArchiveInstanceInfo](../)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* assembly [Aspose.Zip](../../../)


