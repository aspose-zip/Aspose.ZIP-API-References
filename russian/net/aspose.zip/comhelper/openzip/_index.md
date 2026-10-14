---
title: "ComHelper.OpenZip"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод ComHelper. Позволяет COM‑приложению загрузить ZIP‑архив из потока."
type: docs
weight: 50
url: /ru/net/aspose.zip/comhelper/openzip/
---
## OpenZip(Stream) {#openzip}

Позволяет COM‑приложению загрузить ZIP‑архив из потока.

```csharp
public Archive OpenZip(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Объект .NET‑потока, содержащий архив для загрузки. |

### Возвращаемое значение

Объект [`Archive`](../../archive/), представляющий архив.

### Исключения

| исключение | условие |
| --- | --- |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |

### См. также

* class [Archive](../../archive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)

---

## OpenZip(string) {#openzip_1}

Позволяет COM‑приложению загрузить ZIP‑архив из файла.

```csharp
public Archive OpenZip(string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | Имя файла архива для загрузки. |

### Возвращаемое значение

Объект [`Archive`](../../archive/), представляющий архив.

### Исключения

| исключение | условие |
| --- | --- |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| ArgumentException | Имя файла пустое, содержит только пробелы или содержит недопустимые символы. |
| ArgumentNullException | *fileName* равно `null`. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| FileNotFoundException | Файл не найден. |
| PathTooLongException | Указанный путь, имя файла или их комбинация превышают системно определённую максимальную длину. |
| UnauthorizedAccessException | Доступ к *fileName* запрещён. |

### См. также

* class [Archive](../../archive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)


