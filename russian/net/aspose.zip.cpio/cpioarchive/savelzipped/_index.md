---
title: "CpioArchive.SaveLzipped"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод CpioArchive. Сохраняет архив в поток с lzip‑сжатием."
type: docs
weight: 100
url: /ru/net/aspose.zip.cpio/cpioarchive/savelzipped/
---
## SaveLzipped(Stream, CpioFormat) {#savelzipped}

Сохраняет архив в поток с lzip‑сжатием.

```csharp
public void SaveLzipped(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
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
using (FileStream result = File.OpenWrite("result.cpio.lz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
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

## SaveLzipped(string, CpioFormat) {#savelzipped_1}

Сохраняет архив в файл по пути с lzip‑сжатием.

```csharp
public void SaveLzipped(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан. |
| cpioFormat | CpioFormat | Определяет формат заголовка cpio. |

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| ArgumentException | *path* является строкой нулевой длины, содержит только пробелы или содержит один или несколько недопустимых символов, определённых в InvalidPathChars. |
| ArgumentNullException | *path* равно `null`. |
| DirectoryNotFoundException | Указанный путь недействителен (например, он находится на не смонтированном диске). |
| IOException | Произошла ошибка ввода/вывода. |
| PathTooLongException | Указанный путь, имя файла или их комбинация превышают системно определённую максимальную длину. |
| UnauthorizedAccessException | У вызывающего нет необходимого разрешения. -или- *path* указывает на файл или каталог только для чтения. |

## Примеры

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.cpio.lz");
    }
}
```

### См. также

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


