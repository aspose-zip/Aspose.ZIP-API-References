---
title: "Archive.CreateEntries"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод архива. Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога."
type: docs
weight: 50
url: /ru/net/aspose.zip/archive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога.

```csharp
public Archive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
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
| DirectoryNotFoundException | Путь к *directory* недействителен, например, находится на несвязанном диске. |
| SecurityException | Вызвавший процесс не имеет необходимого разрешения для доступа к *directory*. |
| ObjectDisposedException | Выбрасывается, если архив был освобождён. |
| ArgumentNullException | *directory* равен `null`. |

## Примеры

```csharp
using (Archive archive = new Archive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.zip");
}
```

### См. также

* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога.

```csharp
public Archive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
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
| ObjectDisposedException | Выбрасывается, если архив был освобождён. |
| ArgumentException | *sourceDirectory* содержит недопустимые символы, такие как ", &lt;, &gt;, или &#x7C;. |
| ArgumentNullException | *sourceDirectory* равно `null`. |
| PathTooLongException | Указанный путь, имя файла или их комбинация превышают системно определённую максимальную длину. |

## Примеры

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.zip");
}
```

### См. также

* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


