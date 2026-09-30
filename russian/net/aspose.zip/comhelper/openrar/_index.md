---
title: "ComHelper.OpenRar"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод ComHelper. Позволяет COM‑приложению загрузить rar‑архив из потока"
type: docs
weight: 40
url: /ru/net/aspose.zip/comhelper/openrar/
---
## OpenRar(Stream) {#openrar}

Позволяет COM‑приложению загрузить rar‑архив из потока.

```csharp
public RarArchive OpenRar(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Объект .NET‑потока, содержащий архив для загрузки. |

### Возвращаемое значение

Объект [`RarArchive`](../../../aspose.zip.rar/rararchive/), представляющий архив.

### Исключения

| исключение | условие |
| --- | --- |
| InvalidDataException | Выбрасывается, когда данные недействительны или повреждены. |

### См. также

* class [RarArchive](../../../aspose.zip.rar/rararchive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)

---

## OpenRar(string) {#openrar_1}

Позволяет COM‑приложению загрузить rar‑архив из файла.

```csharp
public RarArchive OpenRar(string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | Имя файла архива для загрузки. |

### Возвращаемое значение

Объект [`RarArchive`](../../../aspose.zip.rar/rararchive/), представляющий архив.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | Имя файла пустое, содержит только пробелы или содержит недопустимые символы. |
| ArgumentNullException | *fileName* равно `null`. |
| Exception | Выбрасывается, когда происходит ошибка выполнения. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| FileNotFoundException | Файл не найден. |
| InvalidDataException | Выбрасывается, когда данные недействительны или повреждены. |
| PathTooLongException | Указанный путь, имя файла или их комбинация превышают системно определённую максимальную длину. |
| UnauthorizedAccessException | Доступ к *fileName* запрещён. |

### См. также

* class [RarArchive](../../../aspose.zip.rar/rararchive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)


