---
title: "SplitSevenZipArchiveSaveOptions.SplitSevenZipArchiveSaveOptions"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор SplitSevenZipArchiveSaveOptions. Создаёт настройки для сохранения многотомного архива 7z"
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/splitsevenziparchivesaveoptions/splitsevenziparchivesaveoptions/
---
## SplitSevenZipArchiveSaveOptions constructor

Создаёт параметры для сохранения многотомного 7z‑архива.

```csharp
public SplitSevenZipArchiveSaveOptions(string fileName, uint segmentSize)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | Имя томов. Может быть с расширением .7z или без него. |
| segmentSize | UInt32 | Размер тома. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | *segmentSize* меньше 100. |

## Примечания

Некоторые тома могут быть меньше *segmentSize*. В большинстве случаев последний сегмент будет меньше, но иногда обычные сегменты тоже могут быть меньше.

Имена файлов будут следующими: *fileName*.7z.001, *fileName*.7z.002, ..., *fileName*.7z.(n).

### См. также

* class [SplitSevenZipArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../splitsevenziparchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


