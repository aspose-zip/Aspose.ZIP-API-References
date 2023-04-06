---
title: TarArchive.SaveZCompressed
second_title: Aspose.ZIP для справочника API .NET
description: TarArchive метод. Сохраняет архив в поток с Zсжатием.
type: docs
weight: 160
url: /ru/net/aspose.zip.tar/tararchive/savezcompressed/
---
## SaveZCompressed(Stream, TarFormat?) {#savezcompressed}

Сохраняет архив в поток с Z-сжатием.

```csharp
public void SaveZCompressed(Stream output, TarFormat? format = default)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| output | Stream | Целевой поток. |
| format | Nullable`1 | Определяет формат заголовка tar. Нулевое значение будет рассматриваться как USTar, когда это возможно. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *output* нулевой. |
| ArgumentException | *output* не доступен для записи. |

### Примечания

*output*должен быть доступен для записи.

### Примеры

```csharp
using (FileStream result = File.OpenWrite("result.tar.Z"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZCompressed(result);
        }
    }
}
```

### Смотрите также

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* пространство имен [Aspose.Zip.Tar](../../tararchive/)
* сборка [Aspose.Zip](../../../)

---

## SaveZCompressed(string, TarFormat?) {#savezcompressed_1}

Сохраняет архив в путь по пути с Z-сжатием.

```csharp
public void SaveZCompressed(string path, TarFormat? format = default)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь создаваемого архива. Если указанное имя файла указывает на существующий файл, он будет перезаписан. |
| format | Nullable`1 | Определяет формат заголовка tar. Нулевое значение будет рассматриваться как USTar, когда это возможно. |

### Примеры

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZCompressed("result.tar.Z");
    }
}
```

### Смотрите также

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* пространство имен [Aspose.Zip.Tar](../../tararchive/)
* сборка [Aspose.Zip](../../../)


