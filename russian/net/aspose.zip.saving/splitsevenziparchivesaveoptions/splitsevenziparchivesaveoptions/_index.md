---
title: SplitSevenZipArchiveSaveOptions.SplitSevenZipArchiveSaveOptions
second_title: Aspose.ZIP для справочника API .NET
description: SplitSevenZipArchiveSaveOptions строитель. Задает настройки для сохранения многотомного архива 7z.
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/splitsevenziparchivesaveoptions/splitsevenziparchivesaveoptions/
---
## SplitSevenZipArchiveSaveOptions constructor

Задает настройки для сохранения многотомного архива 7z.

```csharp
public SplitSevenZipArchiveSaveOptions(string fileName, uint segmentSize)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | Имя для томов. Может быть с расширением .7z или без него. |
| segmentSize | UInt32 | Размер тома. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | *segmentSize* меньше 100. |

### Примечания

Некоторые объемы могут быть меньше*segmentSize*. В большинстве случаев последний сегмент будет меньше, но редко могут быть и обычные сегменты.

Имена файлов будут следующими:*fileName* .7з.001,*fileName* .7з.002,...,*fileName*.7з.(н).

### Смотрите также

* class [SplitSevenZipArchiveSaveOptions](../)
* пространство имен [Aspose.Zip.Saving](../../splitsevenziparchivesaveoptions/)
* сборка [Aspose.Zip](../../../)


