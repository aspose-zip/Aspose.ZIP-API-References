---
title: "XarBzip2CompressionSettings.XarBzip2CompressionSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор XarBzip2CompressionSettings. Инициализирует новый экземпляр класса XarBzip2CompressionSettings"
type: docs
weight: 10
url: /ru/net/aspose.zip.xar/xarbzip2compressionsettings/xarbzip2compressionsettings/
---
## XarBzip2CompressionSettings(int) {#constructor_1}

Инициализирует новый экземпляр класса [`XarBzip2CompressionSettings`](../).

```csharp
public XarBzip2CompressionSettings(int blockSize)
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
using (XarArchive archive = new XarArchive())
{
    archive.CreateEntry("data.bin", "data.bin", new XarBzip2CompressionSettings(1));
    archive.Save("archive.xar");
}
```

### См. также

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## XarBzip2CompressionSettings() {#constructor}

Инициализирует новый экземпляр класса [`XarBzip2CompressionSettings`](../) с размером блока по умолчанию, равным 9 сотням килобайт.

```csharp
public XarBzip2CompressionSettings()
```

### См. также

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)


