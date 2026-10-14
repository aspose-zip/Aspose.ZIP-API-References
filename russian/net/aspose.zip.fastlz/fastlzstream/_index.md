---
title: "Класс FastLZStream"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.FastLZ.FastLZStream. Обёртка потока, которая сжимает данные с помощью FastLZ. Реализует шаблон декоратора."
type: docs
weight: 500
url: /ru/net/aspose.zip.fastlz/fastlzstream/
---
## FastLZStream class

Обёртка потока, которая сжимает данные с помощью FastLZ. Реализует шаблон декоратора.

```csharp
public class FastLZStream : Stream
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [FastLZStream](fastlzstream/)(Stream, int) | Инициализирует новый экземпляр класса `FastLZStream`, подготовленный для сжатия. |

## Свойства

| Имя | Описание |
| --- | --- |
| override [CanRead](../../aspose.zip.fastlz/fastlzstream/canread/) { get; } | Возвращает значение, указывающее, поддерживает ли текущий поток чтение. |
| override [CanSeek](../../aspose.zip.fastlz/fastlzstream/canseek/) { get; } | Возвращает значение, указывающее, поддерживает ли текущий поток перемещение позиции. |
| override [CanWrite](../../aspose.zip.fastlz/fastlzstream/canwrite/) { get; } | Возвращает значение, указывающее, поддерживает ли текущий поток запись. |
| override [Length](../../aspose.zip.fastlz/fastlzstream/length/) { get; } | Возвращает длину потока в байтах. |
| override [Position](../../aspose.zip.fastlz/fastlzstream/position/) { get; set; } | Получает или задаёт позицию в текущем потоке. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Close](../../aspose.zip.fastlz/fastlzstream/close/)() | Закрывает текущий поток и освобождает любые ресурсы (например, сокеты и файловые дескрипторы), связанные с текущим потоком. |
| override [Flush](../../aspose.zip.fastlz/fastlzstream/flush/)() | Очищает все буферы этого потока и заставляет любые буферизованные данные записаться в нижележащее устройство. |
| override [Read](../../aspose.zip.fastlz/fastlzstream/read/)(byte[], int, int) | Читает последовательность байтов из потока и перемещает позицию в потоке на количество прочитанных байтов. Не поддерживается. |
| override [Seek](../../aspose.zip.fastlz/fastlzstream/seek/)(long, SeekOrigin) | Устанавливает позицию в текущем потоке. |
| override [SetLength](../../aspose.zip.fastlz/fastlzstream/setlength/)(long) | Устанавливает длину текущего потока. |
| override [Write](../../aspose.zip.fastlz/fastlzstream/write/)(byte[], int, int) | Записывает последовательность байтов в сжимающий поток и перемещает текущую позицию в этом потоке на количество записанных байтов. |

### См. также

* namespace [Aspose.Zip.FastLZ](../../aspose.zip.fastlz/)
* assembly [Aspose.Zip](../../)


