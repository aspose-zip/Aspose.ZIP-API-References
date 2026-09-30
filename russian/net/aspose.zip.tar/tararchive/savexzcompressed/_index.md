---
title: "TarArchive.SaveXzCompressed"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод TarArchive. Сохраняет архив в поток с xz‑сжатием"
type: docs
weight: 200
url: /ru/net/aspose.zip.tar/tararchive/savexzcompressed/
---
## SaveXzCompressed(Stream, TarFormat?, XzArchiveSettings) {#savexzcompressed}

Сохраняет архив в поток с xz‑сжатием.

```csharp
public void SaveXzCompressed(Stream output, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| output | Stream | Поток назначения. |
| формат | Nullable`1 | Определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно. |
| настройки | XzArchiveSettings | Набор параметров конкретного xz‑архива: размер словаря, размер блока, тип проверки. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *output* равен null. |
| ArgumentException | *output* не доступен для записи. |
| ObjectDisposedException | Архив был освобождён и не может быть использован |
| IOException | Произошла ошибка ввода/вывода. |

## Примечания

*output*The stream must be writable.

## Примеры

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

### См. также

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, TarFormat?, XzArchiveSettings) {#savexzcompressed_1}

Сохраняет архив по указанному пути с xz‑сжатием.

```csharp
public void SaveXzCompressed(string path, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан. |
| формат | Nullable`1 | Определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно. |
| настройки | XzArchiveSettings | Набор параметров конкретного xz‑архива: размер словаря, размер блока, тип проверки. |

### Исключения

| исключение | условие |
| --- | --- |
| UnauthorizedAccessException | У вызывающего нет необходимого разрешения. -или- *path* указывает на файл или каталог только для чтения. |
| ArgumentException | *path* является строкой нулевой длины, содержит только пробелы или содержит один или несколько недопустимых символов, определённых в InvalidPathChars. |
| ArgumentNullException | *path* имеет значение null. |
| PathTooLongException | Указанный *path*, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. |
| DirectoryNotFoundException | Указанный *path* недействителен (например, находится на неподключённом диске). |
| NotSupportedException | *path* имеет недопустимый формат. |
| ObjectDisposedException | Архив был освобождён и не может быть использован |
| IOException | Произошла ошибка ввода/вывода. |

## Примеры

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

### См. также

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


