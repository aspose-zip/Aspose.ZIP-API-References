---
title: "ComHelper.OpenBzip2"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод ComHelper. Позволяет COM‑приложению загрузить bzip2‑архив из потока"
type: docs
weight: 20
url: /ru/net/aspose.zip/comhelper/openbzip2/
---
## OpenBzip2(Stream) {#openbzip2}

Позволяет COM‑приложению загрузить архив bzip2 из потока.

```csharp
public Bzip2Archive OpenBzip2(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Объект .NET‑потока, содержащий архив для загрузки. |

### Возвращаемое значение

Объект [`Bzip2Archive`](../../../aspose.zip.bzip2/bzip2archive/), представляющий архив.

### Исключения

| исключение | условие |
| --- | --- |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| InvalidDataException | Неправильные байты сигнатуры. |

### См. также

* class [Bzip2Archive](../../../aspose.zip.bzip2/bzip2archive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)

---

## OpenBzip2(string) {#openbzip2_1}

Позволяет COM‑приложению загрузить архив bzip2 из файла.

```csharp
public Bzip2Archive OpenBzip2(string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | Имя файла архива для загрузки. |

### Возвращаемое значение

Объект [`Bzip2Archive`](../../../aspose.zip.bzip2/bzip2archive/), представляющий архив.

### Исключения

| исключение | условие |
| --- | --- |
| EndOfStreamException | Выбрасывается, когда конец потока достигается до чтения ожидаемого количества байтов. |
| ArgumentException | Имя файла пустое, содержит только пробелы или содержит недопустимые символы. |
| ArgumentNullException | *fileName* равно `null`. |
| DirectoryNotFoundException | Указанный путь недействителен, например, находится на не смонтированном диске. |
| FileNotFoundException | Файл не найден. |
| InvalidDataException | Неправильные байты сигнатуры. |
| PathTooLongException | Указанный путь, имя файла или их комбинация превышают системно определённую максимальную длину. |
| UnauthorizedAccessException | Доступ к *fileName* запрещён. |

### См. также

* class [Bzip2Archive](../../../aspose.zip.bzip2/bzip2archive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)


