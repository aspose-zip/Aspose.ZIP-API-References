---
title: "Bzip2CompressionSettings.Bzip2CompressionSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Bzip2CompressionSettings конструктор. Инициализирует новый экземпляр класса Bzip2CompressionSettings"
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/bzip2compressionsettings/bzip2compressionsettings/
---
## Bzip2CompressionSettings(int) {#constructor_1}

Инициализирует новый экземпляр класса [`Bzip2CompressionSettings`](../).

```csharp
public Bzip2CompressionSettings(int blockSize)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| blockSize | Int32 | Размер блока в сотнях килобайт. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | Размер блока не находится в диапазоне от 1 до 9. |

## Примеры

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### См. также

* class [Bzip2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## Bzip2CompressionSettings() {#constructor}

Инициализирует новый экземпляр класса [`Bzip2CompressionSettings`](../) с размером блока по умолчанию, равным 9 сотням килобайт.

```csharp
public Bzip2CompressionSettings()
```

## Примеры

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### См. также

* class [Bzip2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)


