---
title: SevenZipArchive.SaveSplit
second_title: Aspose.ZIP для справочника API .NET
description: SevenZipArchive метод. Сохраняет многотомный архив в указанный каталог назначения.
type: docs
weight: 90
url: /ru/net/aspose.zip.sevenzip/sevenziparchive/savesplit/
---
## SevenZipArchive.SaveSplit method

Сохраняет многотомный архив в указанный каталог назначения.

```csharp
public void SaveSplit(string destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationDirectory | String | Путь к каталогу, в котором будут создаваться сегменты архива. |
| options | SplitSevenZipArchiveSaveOptions | Варианты сохранения архива, включая имя файла. |

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Этот архив был открыт из существующего источника. |
| ArgumentNullException | *destinationDirectory* нулевой. |
| SecurityException | У вызывающего абонента нет необходимого разрешения для доступа к каталогу. |
| ArgumentException | *destinationDirectory* содержит недопустимые символы, такие как ", &gt;, &lt; или &#x7C;. |
| PathTooLongException | Указанный путь превышает максимальную длину, определенную системой. |

### Примечания

Этот метод состоит из нескольких (`н`) файлы имя_файла.7z.001, имя_файла.7z.002, ..., имя_файла.7z.(n).

Невозможно сделать существующий архив многотомным.

### Примеры

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitSevenZipArchiveSaveOptions("volume", 65536));
}
```

### Смотрите также

* class [SplitSevenZipArchiveSaveOptions](../../../aspose.zip.saving/splitsevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* пространство имен [Aspose.Zip.SevenZip](../../sevenziparchive/)
* сборка [Aspose.Zip](../../../)


