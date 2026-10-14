---
title: "CpioArchive.SaveXzCompressed"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод CpioArchive. Сохраняет архив в поток с xz‑сжатием."
type: docs
weight: 120
url: /ru/net/aspose.zip.cpio/cpioarchive/savexzcompressed/
---
## SaveXzCompressed(Stream, CpioFormat, XzArchiveSettings) {#savexzcompressed}

Сохраняет архив в поток с xz‑сжатием.

```csharp
public void SaveXzCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| output | Stream | Поток назначения. |
| cpioFormat | CpioFormat | Определяет формат заголовка cpio. |
| настройки | XzArchiveSettings | Набор параметров конкретного xz‑архива: размер словаря, размер блока, тип проверки. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *output* равен null. |
| ArgumentException | *output* не доступен для записи. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примечания

*output*The stream must be writable.

## Примеры

```csharp
using (FileStream result = File.OpenWrite("result.cpio.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### См. также

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, CpioFormat, XzArchiveSettings) {#savexzcompressed_1}

Сохраняет архив по указанному пути с xz‑сжатием.

```csharp
public void SaveXzCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан. |
| cpioFormat | CpioFormat | Определяет формат заголовка cpio. |
| настройки | XzArchiveSettings | Набор параметров конкретного xz‑архива: размер словаря, размер блока, тип проверки. |

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| ArgumentNullException | *path* равно `null`. |
| IOException | Произошла ошибка ввода/вывода. |
| InvalidDataException | Выбрасывается, когда данные недействительны или повреждены. |
| PathTooLongException | Указанный путь, имя файла или их комбинация превышают системно определённую максимальную длину. |

## Примеры

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.cpio.xz");
    }
}
```

### См. также

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


