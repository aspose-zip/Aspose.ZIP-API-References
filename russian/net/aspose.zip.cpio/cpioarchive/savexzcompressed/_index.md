---
title: CpioArchive.SaveXzCompressed
second_title: Aspose.ZIP для справочника API .NET
description: CpioArchive метод. Сохраняет архив в поток со сжатием xz.
type: docs
weight: 100
url: /ru/net/aspose.zip.cpio/cpioarchive/savexzcompressed/
---
## SaveXzCompressed(Stream, CpioFormat, XzArchiveSettings) {#savexzcompressed}

Сохраняет архив в поток со сжатием xz.

```csharp
public void SaveXzCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| output | Stream | Целевой поток. |
| cpioFormat | CpioFormat | Определяет формат заголовка cpio. |
| settings | XzArchiveSettings | Набор настроек конкретного архива xz: размер словаря, размер блока, тип проверки. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *output* нулевой. |
| ArgumentException | *output* не доступен для записи. |

### Примечания

*output*Поток должен быть доступен для записи.

### Примеры

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

### Смотрите также

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* пространство имен [Aspose.Zip.Cpio](../../cpioarchive/)
* сборка [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, CpioFormat, XzArchiveSettings) {#savexzcompressed_1}

Сохраняет архив в путь по пути со сжатием xz.

```csharp
public void SaveXzCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь создаваемого архива. Если указанное имя файла указывает на существующий файл, он будет перезаписан. |
| cpioFormat | CpioFormat | Определяет формат заголовка cpio. |
| settings | XzArchiveSettings | Набор настроек конкретного архива xz: размер словаря, размер блока, тип проверки. |

### Примеры

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

### Смотрите также

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* пространство имен [Aspose.Zip.Cpio](../../cpioarchive/)
* сборка [Aspose.Zip](../../../)


