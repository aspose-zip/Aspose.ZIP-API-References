---
title: "XarArchive.CreateEntries"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод XarArchive. Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога"
type: docs
weight: 30
url: /ru/net/aspose.zip.xar/xararchive/createentries/
---
## CreateEntries(string, bool, XarCompressionSettings) {#createentries_1}

Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога.

```csharp
public XarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceDirectory | String | Каталог для сжатия. |
| compressionSettings | Boolean | Настройки сжатия, используемые для добавленных элементов [`XarEntry`](../../xarentry/). |
| includeRootDirectory | XarCompressionSettings | Указывает, включать ли корневой каталог сам по себе. |

### Возвращаемое значение

Экземпляр записи Xar.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *sourceDirectory* имеет значение null. |
| SecurityException | У вызывающего нет необходимого разрешения для доступа к *sourceDirectory*. |
| ArgumentException | *sourceDirectory* содержит недопустимые символы, такие как ", &lt;, &gt;, или &#x7C;. |
| PathTooLongException | Указанный путь, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. Указанный путь, имя файла или оба слишком длинные. |
| IOException | *sourceDirectory* обозначает файл, а не каталог. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примеры

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(@"C:\folder", false);
        archive.Save(xarFile);
    }
}
```

### См. также

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool, XarCompressionSettings) {#createentries}

Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога.

```csharp
public XarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| directory | DirectoryInfo | Каталог для сжатия. |
| compressionSettings | Boolean | Настройки сжатия, используемые для добавленных элементов [`XarEntry`](../../xarentry/). |
| includeRootDirectory | XarCompressionSettings | Указывает, включать ли корневой каталог сам по себе. |

### Возвращаемое значение

Экземпляр записи Xar.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *directory* равно null. |
| SecurityException | Вызвавший процесс не имеет необходимого разрешения для доступа к *directory*. |
| IOException | *directory* обозначает файл, а не каталог. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примеры

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(new DirectoryInfo(@"C:\folder"), false);
        archive.Save(xarFile);
    }
}
```

### См. также

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


