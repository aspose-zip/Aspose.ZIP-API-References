---
title: "SharArchive.CreateEntries"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод SharArchive. Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога"
type: docs
weight: 30
url: /ru/net/aspose.zip.shar/shararchive/createentries/
---
## CreateEntries(string, bool) {#createentries_1}

Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога.

```csharp
public SharArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceDirectory | String | Каталог для сжатия. |
| includeRootDirectory | Boolean | Указывает, включать ли корневой каталог сам по себе. |

### Возвращаемое значение

Экземпляр элемента Shar.

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
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(sharFile);
    }
}
```

### См. также

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool) {#createentries}

Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога.

```csharp
public SharArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| directory | DirectoryInfo | Каталог для сжатия. |
| includeRootDirectory | Boolean | Указывает, включать ли корневой каталог сам по себе. |

### Возвращаемое значение

Экземпляр элемента Shar.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *directory* равно null. |
| SecurityException | Вызвавший процесс не имеет необходимого разрешения для доступа к *directory*. |
| IOException | *directory* обозначает файл, а не каталог. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примеры

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(sharFile);
    }
}
```

### См. также

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


