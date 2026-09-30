---
title: "CpioArchive.CreateEntries"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод CpioArchive. Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога."
type: docs
weight: 30
url: /ru/net/aspose.zip.cpio/cpioarchive/createentries/
---
## CreateEntries(string, bool) {#createentries_1}

Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога.

```csharp
public CpioArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceDirectory | String | Каталог для сжатия. |
| includeRootDirectory | Boolean | Указывает, включать ли корневой каталог сам по себе. |

### Возвращаемое значение

Экземпляр записи Cpio.

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
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(cpioFile);
    }
}
```

### См. также

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool) {#createentries}

Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога.

```csharp
public CpioArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| directory | DirectoryInfo | Каталог для сжатия. |
| includeRootDirectory | Boolean | Указывает, включать ли корневой каталог сам по себе. |

### Возвращаемое значение

Экземпляр записи Cpio.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *directory* равно null. |
| SecurityException | Вызвавший процесс не имеет необходимого разрешения для доступа к *directory*. |
| IOException | *directory* обозначает файл, а не каталог. |
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |

## Примеры

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(cpioFile);
    }
}
```

### См. также

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


