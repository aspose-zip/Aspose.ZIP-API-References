---
title: "CpioArchive.SaveLZMACompressed"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод CpioArchive. Сохраняет архив в поток с компрессией LZMA."
type: docs
weight: 110
url: /ru/net/aspose.zip.cpio/cpioarchive/savelzmacompressed/
---
## SaveLZMACompressed(Stream, CpioFormat) {#savelzmacompressed}

Сохраняет архив в поток с компрессией LZMA.

```csharp
public void SaveLZMACompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| output | Stream | Поток назначения. |
| cpioFormat | CpioFormat | Определяет формат заголовка cpio. |

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| NotSupportedException | Поток не поддерживает запись, или поток уже закрыт. |

## Примечания

*output* must be writable.

Важно: cpio‑архив создаётся, а затем сжимается в этом методе, его содержимое хранится внутри. Будьте внимательны к потреблению памяти.

## Примеры

```csharp
using (FileStream result = File.OpenWrite("result.cpio.lzma"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZMACompressed(result);
        }
    }
}
```

### См. также

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLZMACompressed(string, CpioFormat) {#savelzmacompressed_1}

Сохраняет архив в файл по пути с компрессией lzma.

```csharp
public void SaveLZMACompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан. |
| cpioFormat | CpioFormat | Определяет формат заголовка cpio. |

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| ArgumentNullException | *path* равно `null`. |
| Exception | Выбрасывается, когда происходит ошибка выполнения. |
| DirectoryNotFoundException | Указанный путь недействителен (например, он находится на не смонтированном диске). |
| IOException | Произошла ошибка ввода/вывода. |
| PathTooLongException | Указанный путь, имя файла или их комбинация превышают системно определённую максимальную длину. |
| UnauthorizedAccessException | У вызывающего нет необходимого разрешения. -или- *path* указывает на файл или каталог только для чтения. |

## Примечания

Важно: cpio‑архив создаётся, а затем сжимается в этом методе, его содержимое хранится внутри. Будьте внимательны к потреблению памяти.

## Примеры

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZMACompressed("result.cpio.lzma");
    }
}
```

### См. также

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


