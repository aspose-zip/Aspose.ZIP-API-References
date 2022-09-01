---
title: SaveXzCompressed
second_title: Aspose.ZIP для справочника API .NET
description: Сохраняет архив в поток со сжатием xz.
type: docs
weight: 150
url: /ru/net/aspose.zip.tar/tararchive/savexzcompressed/
---
## SaveXzCompressed(Stream, TarFormat?, XzArchiveSettings) {#savexzcompressed}

Сохраняет архив в поток со сжатием xz.

```csharp
public void SaveXzCompressed(Stream output, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| output | Stream | Целевой поток. |
| format | Nullable`1 | Определяет формат заголовка tar. Нулевое значение будет рассматриваться как USTar, когда это возможно. |
| settings | XzArchiveSettings | Набор настроек конкретного архива xz:размер словаря, размер блока, тип проверки. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *output*равно нулю. |
| ArgumentException | *output*недоступен для записи. |

### Примечания

*output*Поток должен быть доступен для записи.

### Примеры

```csharp
using (FileStream result = File.OpenWrite("result.tar.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### Смотрите также

* enum [TarFormat](../../tarformat)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings)
* class [TarArchive](../../tararchive)
* пространство имен [Aspose.Zip.Tar](../../tararchive)
* сборка [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, TarFormat?, XzArchiveSettings) {#savexzcompressed_1}

Сохраняет архив в путь по пути со сжатием xz.

```csharp
public void SaveXzCompressed(string path, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь создаваемого архива. Если указанное имя файла указывает на существующий файл, он будет перезаписан. |
| format | Nullable`1 | Определяет формат заголовка tar. Нулевое значение будет рассматриваться как USTar, когда это возможно. |
| settings | XzArchiveSettings | Набор настроек конкретного архива xz:размер словаря, размер блока, тип проверки. |

### Примеры

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.tar.xz");
    }
}
```

### Смотрите также

* enum [TarFormat](../../tarformat)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings)
* class [TarArchive](../../tararchive)
* пространство имен [Aspose.Zip.Tar](../../tararchive)
* сборка [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->