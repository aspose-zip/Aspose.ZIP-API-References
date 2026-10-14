---
title: "SplitArchiveSaveOptions.SplitArchiveSaveOptions"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор SplitArchiveSaveOptions. Создаёт параметры для сохранения многотомного ZIP‑архива."
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/splitarchivesaveoptions/splitarchivesaveoptions/
---
## SplitArchiveSaveOptions(string, uint) {#constructor}

Создает экземпляр настроек для сохранения многотомного ZIP-архива.

```csharp
public SplitArchiveSaveOptions(string fileName, uint segmentSize)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | Имя томов. Может быть с расширением .zip или без него. |
| segmentSize | UInt32 | Размер тома. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | Размер сегмента меньше 65536 байт. |

## Примечания

Некоторые тома могут быть меньше *segmentSize*. В большинстве случаев последний сегмент будет меньше, но иногда обычные сегменты тоже могут быть меньше.

Имена файлов будут следующими: *fileName*.z01, *fileName*.z02, ..., *fileName*.z(n-1), *fileName*.zip.

### См. также

* class [SplitArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)

---

## SplitArchiveSaveOptions(uint) {#constructor_1}

Создает экземпляр настроек для сохранения многотомного ZIP-архива.

```csharp
public SplitArchiveSaveOptions(uint segmentSize)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| segmentSize | UInt32 | Размер тома. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | Размер сегмента меньше 65536 байт. |

## Примечания

Используйте этот экземпляр `SplitArchiveSaveOptions` без имени файла с методом [`SaveSplit`](../../../aspose.zip/archive/savesplit/).

Некоторые тома могут быть меньше *segmentSize*. В большинстве случаев последний сегмент будет меньше, но иногда обычные сегменты тоже могут быть меньше.

### См. также

* class [SplitArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


