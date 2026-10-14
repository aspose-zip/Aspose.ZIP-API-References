---
title: "IsoEntry.Extract"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод IsoEntry. Извлекает элемент в файловую систему по указанному пути"
type: docs
weight: 50
url: /ru/net/aspose.zip.iso/isoentry/extract/
---
## Extract(string) {#extract}

Извлекает запись в файловую систему по указанному пути.

```csharp
public FileInfo Extract(string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к целевому файлу. Если файл уже существует, он будет перезаписан. |

### Возвращаемое значение

Экземпляр FileInfo, содержащий извлечённые данные.

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
| InvalidOperationException | Заголовки архива и служебная информация не были прочитаны. |

### См. также

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Извлекает запись в предоставленный поток.

```csharp
public void Extract(Stream destination)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | Stream | Поток назначения. Должен поддерживать запись. |

### Исключения

| исключение | условие |
| --- | --- |
| NotSupportedException | Выбрасывается, если элемент не представляет файл. |
| ArgumentException | Указанный поток не поддерживает запись. |

### См. также

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
* assembly [Aspose.Zip](../../../)


