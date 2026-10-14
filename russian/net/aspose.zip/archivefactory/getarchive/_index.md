---
title: "ArchiveFactory.GetArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод ArchiveFactory. Определяет формат архива и создает соответствующий объект IArchive в соответствии с типом архива, указанным в заданном пути"
type: docs
weight: 20
url: /ru/net/aspose.zip/archivefactory/getarchive/
---
## GetArchive(string) {#getarchive_2}

Определяет формат архива и создает соответствующий объект [`IArchive`](../../iarchive/) в соответствии с типом архива, указанным в заданном пути.

```csharp
public static IArchive GetArchive(string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к архиву, который будет проанализирован. |

### Возвращаемое значение

Объект [`IArchive`](../../iarchive/), представляющий архив.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *path* равно `null`. |
| DirectoryNotFoundException | Указанный путь недействителен (например, он находится на не смонтированном диске). |
| FileNotFoundException | Файл, указанный в *path*, не найден. |
| IOException | Во время открытия файла произошла ошибка ввода/вывода. |
| PathTooLongException | Указанный путь, имя файла или их комбинация превышают системно определённую максимальную длину. |
| UnauthorizedAccessException | *path* указывает на каталог. -или- У вызывающего нет необходимых прав. |

### См. также

* interface [IArchive](../../iarchive/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)

---

## GetArchive(Stream) {#getarchive}

Определяет формат архива и создает соответствующий объект [`IArchive`](../../iarchive/) в соответствии с типом архива, указанным в заданном потоке.

```csharp
public static IArchive GetArchive(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Поток, содержащий данные архива. Он должен поддерживать перемещение. |

### Возвращаемое значение

Объект [`IArchive`](../../iarchive/), представляющий архив.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *stream* не поддерживает поиск. |
| ArgumentNullException | *stream* равно null. |

### См. также

* interface [IArchive](../../iarchive/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)

---

## GetArchive(Stream, string) {#getarchive_1}

Определяет формат архива и создает соответствующий объект [`IArchive`](../../iarchive/) в соответствии с типом зашифрованного архива, указанного в заданном потоке.

```csharp
public static IArchive GetArchive(Stream stream, string password)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Поток, содержащий данные архива. Он должен поддерживать перемещение. |
| password | String | Пароль для расшифровки зашифрованного архива. |

### Возвращаемое значение

Объект [`IArchive`](../../iarchive/), представляющий архив.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | *stream* не поддерживает поиск. |
| ArgumentNullException | *stream* равно null. |

### См. также

* interface [IArchive](../../iarchive/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)


