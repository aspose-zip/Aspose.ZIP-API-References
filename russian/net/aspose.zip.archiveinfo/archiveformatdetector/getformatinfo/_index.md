---
title: "GetFormatInfo"
second_title: "Aspose.ZIP for .NET API Справочник"
description: 
type: docs
weight: 20
url: /ru/net/aspose.zip.archiveinfo/archiveformatdetector/getformatinfo/
---
## ArchiveFormatDetector.GetFormatInfo method (1 of 2)

Возвращает информацию о формате.

```csharp
public ArchiveFormatInfo GetFormatInfo(string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | Имя файла архива. |

### Возвращаемое значение

Информация о формате архива или null, если формат не был обнаружен.

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

### См. также

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

---

## ArchiveFormatDetector.GetFormatInfo method (2 of 2)

Возвращает информацию о формате.

```csharp
public ArchiveFormatInfo GetFormatInfo(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Поток архивного файла. |

### Возвращаемое значение

Информация о формате архива или null, если формат не был обнаружен.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *stream* равно null. |
| ArgumentException | *stream* не поддерживает поиск. |

### См. также

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для Aspose.Zip.dll -->
