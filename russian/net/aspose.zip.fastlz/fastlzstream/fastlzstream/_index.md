---
title: "FastLZStream.FastLZStream"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "FastLZStream конструктор. Инициализирует новый экземпляр класса FastLZStream, подготовленный для сжатия"
type: docs
weight: 10
url: /ru/net/aspose.zip.fastlz/fastlzstream/fastlzstream/
---
## FastLZStream constructor

Инициализирует новый экземпляр класса [`FastLZStream`](../) для сжатия.

```csharp
public FastLZStream(Stream stream, int compressionLevel)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Поток для сохранения сжатых данных. |
| compressionLevel | Int32 | Используйте 1 для более быстрого сжатия, используйте 2 для лучшего коэффициента сжатия. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *stream* равно null. |
| ArgumentException | *stream* не поддерживает запись. |
| ArgumentOutOfRangeException | *compressionLevel* больше 2 или меньше 1. |

### См. также

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


