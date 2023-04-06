---
title: SplitArchiveSaveOptions.SplitArchiveSaveOptions
second_title: Aspose.ZIP для справочника API .NET
description: SplitArchiveSaveOptions строитель. Задает настройки для сохранения многотомного zipархива.
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/splitarchivesaveoptions/splitarchivesaveoptions/
---
## SplitArchiveSaveOptions constructor

Задает настройки для сохранения многотомного zip-архива.

```csharp
public SplitArchiveSaveOptions(string fileName, uint segmentSize)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | Имя для томов. Может быть с расширением .zip или без него. |
| segmentSize | UInt32 | Размер тома. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | Размер сегмента меньше 65536 байт. |

### Примечания

Некоторые объемы могут быть меньше*segmentSize*. В большинстве случаев последний сегмент будет меньше, но редко могут быть и обычные сегменты.

Имена файлов будут следующими:*fileName* .z01,*fileName* .z02, ...,*fileName* .z(n-1),*fileName*.zip.

### Смотрите также

* class [SplitArchiveSaveOptions](../)
* пространство имен [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* сборка [Aspose.Zip](../../../)


