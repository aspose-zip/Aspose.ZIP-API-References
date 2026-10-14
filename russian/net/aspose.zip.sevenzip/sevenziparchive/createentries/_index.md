---
title: "SevenZipArchive.CreateEntries"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод SevenZipArchive. Рекурсивно добавляет в архив все файлы и каталоги из указанного каталога."
type: docs
weight: 40
url: /ru/net/aspose.zip.sevenzip/sevenziparchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога.

```csharp
public SevenZipArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
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
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| SecurityException | Вызвавший процесс не имеет необходимого разрешения для доступа к *directory*. |

## Примеры

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.7z");
}
```

### См. также

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога.

```csharp
public SevenZipArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
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
| ObjectDisposedException | Экземпляр архива был освобождён и не может быть использован. |
| ArgumentNullException | *sourceDirectory* равно `null`. |

## Примеры

Создайте 7z‑архив с сжатием LZMA2.

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.7z");
}
```

### См. также

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


