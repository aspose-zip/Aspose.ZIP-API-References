---
title: "TarArchive.SaveGzipped"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод TarArchive. Сохраняет архив в поток с gzip‑сжатием"
type: docs
weight: 160
url: /ru/net/aspose.zip.tar/tararchive/savegzipped/
---
## SaveGzipped(Stream, TarFormat?) {#savegzipped}

Сохраняет архив в поток с gzip‑сжатием.

```csharp
public void SaveGzipped(Stream output, TarFormat? format = default)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| output | Stream | Поток назначения. |
| формат | Nullable`1 | Определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *output* равен null. |
| ArgumentException | *output* не доступен для записи. |
| ObjectDisposedException | Архив был освобождён и не может быть использован |

## Примечания

*output* must be writable.

## Примеры

```csharp
using (FileStream result = File.OpenWrite("result.tar.gz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
        }
    }
}
```

### См. также

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveGzipped(string, TarFormat?) {#savegzipped_1}

Сохраняет архив в файл по пути с gzip‑сжатием.

```csharp
public void SaveGzipped(string path, TarFormat? format = default)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан. |
| формат | Nullable`1 | Определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно. |

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
        archive.SaveGzipped("result.tar.gz");
    }
}
```

### См. также

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


