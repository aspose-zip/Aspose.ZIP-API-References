---
title: Archive.CreateEntries
second_title: Aspose.ZIP для справочника API .NET
description: Archive метод. Добавляет в архив все файлы и каталоги рекурсивно в заданном каталоге.
type: docs
weight: 40
url: /ru/net/aspose.zip/archive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Добавляет в архив все файлы и каталоги рекурсивно в заданном каталоге.

```csharp
public Archive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| directory | DirectoryInfo | Каталог для сжатия. |
| includeRootDirectory | Boolean | Указывает, включать ли сам корневой каталог или нет. |

### Возвращаемое значение

Архив с записями составлен.

### Исключения

| исключение | условие |
| --- | --- |
| DirectoryNotFoundException | Путь к*directory* недействителен, например, находится на несопоставленном диске. |
| SecurityException | У вызывающего абонента нет необходимого разрешения для доступа*directory*. |

### Примеры

```csharp
using (Archive archive = new Archive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.zip");
}
```

### Смотрите также

* class [Archive](../)
* пространство имен [Aspose.Zip](../../archive/)
* сборка [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Добавляет в архив все файлы и каталоги рекурсивно в заданном каталоге.

```csharp
public Archive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceDirectory | String | Каталог для сжатия. |
| includeRootDirectory | Boolean | Указывает, включать ли сам корневой каталог или нет. |

### Возвращаемое значение

Архив с записями составлен.

### Примеры

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.zip");
}
```

### Смотрите также

* class [Archive](../)
* пространство имен [Aspose.Zip](../../archive/)
* сборка [Aspose.Zip](../../../)


