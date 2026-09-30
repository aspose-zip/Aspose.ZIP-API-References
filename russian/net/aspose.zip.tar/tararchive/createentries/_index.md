---
title: "TarArchive.CreateEntries"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод TarArchive. Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога"
type: docs
weight: 100
url: /ru/net/aspose.zip.tar/tararchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога.

```csharp
public TarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| directory | DirectoryInfo | Каталог для сжатия. |
| includeRootDirectory | Boolean | Указывает, включать ли корневой каталог сам по себе. |

### Возвращаемое значение

Архив с составленными записями.

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Архив был освобождён и не может быть использован |

## Примеры

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(tarFile);
    }
}
```

### См. также

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога.

```csharp
public TarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceDirectory | String | Каталог для сжатия. |
| includeRootDirectory | Boolean | Указывает, включать ли корневой каталог сам по себе. |

### Возвращаемое значение

Архив с составленными записями.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *sourceDirectory* имеет значение null. |
| SecurityException | У вызывающего нет необходимого разрешения для доступа к *sourceDirectory*. |
| ArgumentException | *sourceDirectory* содержит недопустимые символы, такие как ", &lt;, &gt;, или &#x7C;. |
| PathTooLongException | Указанный путь, имя файла или оба превышают системно определённую максимальную длину. Например, на платформах Windows пути должны быть короче 248 символов, а имена файлов — короче 260 символов. Указанный путь, имя файла или оба слишком длинные. |
| ObjectDisposedException | Архив был освобождён и не может быть использован |

## Примеры

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(tarFile);
    }
}
```

### См. также

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


