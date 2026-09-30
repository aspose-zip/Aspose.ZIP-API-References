---
title: "ArchiveInstanceInfo.GetArchiveFormatInfo"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод ArchiveInstanceInfo. Получает информацию о формате архива"
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

Информация о формате архива.

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

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* assembly [Aspose.Zip](../../../)

---

## GetArchiveFormatInfo(Stream) {#getarchiveformatinfo}

Получает информацию о формате архива.

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Поток архивного файла. |

### Возвращаемое значение

Информация о формате архива.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *stream* равно null. |
| ArgumentException | *stream* не поддерживает поиск. |

### См. также

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* assembly [Aspose.Zip](../../../)


