---
title: "FastLZStream.Write"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод FastLZStream. Записывает последовательность байтов в сжимающий поток и перемещает текущую позицию в этом потоке на количество записанных байтов."
type: docs
weight: 120
url: /ru/net/aspose.zip.fastlz/fastlzstream/write/
---
## FastLZStream.Write method

Записывает последовательность байтов в сжимающий поток и перемещает текущую позицию в этом потоке на количество записанных байтов.

```csharp
public override void Write(byte[] buffer, int offset, int count)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| buffer | Byte[] | Массив байтов. Этот метод копирует count байтов из buffer в текущий поток. |
| offset | Int32 | Нулевой смещение в байтах в buffer, с которого начинать копирование байтов в текущий поток. |
| count | Int32 | Количество байтов, которое будет записано в текущий поток. |

### Исключения

| исключение | условие |
| --- | --- |
| ObjectDisposedException | Выбрасывается, если поток был освобождён. |
| ArgumentNullException | *buffer* равно `null`. |

### См. также

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


