---
title: "CpioArchive.SaveZCompressed"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод CpioArchive. Сохраняет архив в поток с компрессией Z."
type: docs
weight: 130
url: /ru/net/aspose.zip.cpio/cpioarchive/savezcompressed/
---
## SaveZCompressed(Stream, CpioFormat) {#savezcompressed}

Сохраняет архив в поток с Z‑сжатием.

```csharp
public void SaveZCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| output | Stream | Поток назначения. |
| cpioFormat | CpioFormat | Определяет формат заголовка cpio. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *output* равен null. |
| ArgumentException | *output* не доступен для записи. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примечания

*output* must be writable.

## Примеры

```csharp
using (FileStream result = File.OpenWrite("result.cpio.Z"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZCompressed(result);
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

## SaveZCompressed(string, CpioFormat) {#savezcompressed_1}

Сохраняет архив по указанному пути с Z‑сжатием

```csharp
public void SaveZCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
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
| DirectoryNotFoundException | Указанный путь недействителен (например, он находится на не смонтированном диске). |
| IOException | Произошла ошибка ввода/вывода. |
| PathTooLongException | Указанный путь, имя файла или их комбинация превышают системно определённую максимальную длину. |

## Примеры

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZCompressed("result.cpio.Z");
    }
}
```

### См. также

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


