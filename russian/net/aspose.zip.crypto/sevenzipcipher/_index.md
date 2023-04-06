---
title: Class SevenZipCipher
second_title: Aspose.ZIP для справочника API .NET
description: Aspose.Zip.Crypto.SevenZipCipher сорт. Базовый класс для шифрования AES используемого для шифрования 7zip.
type: docs
weight: 190
url: /ru/net/aspose.zip.crypto/sevenzipcipher/
---
## SevenZipCipher class

Базовый класс для шифрования AES, используемого для шифрования 7-zip.

```csharp
public abstract class SevenZipCipher : ICryptoTransform
```

## Характеристики

| Имя | Описание |
| --- | --- |
| abstract [CanReuseTransform](../../aspose.zip.crypto/sevenzipcipher/canreusetransform/) { get; } | Получает значение, указывающее, можно ли повторно использовать текущее преобразование. |
| abstract [CanTransformMultipleBlocks](../../aspose.zip.crypto/sevenzipcipher/cantransformmultipleblocks/) { get; } | Получает значение, указывающее, можно ли преобразовать несколько блоков. |
| abstract [InputBlockSize](../../aspose.zip.crypto/sevenzipcipher/inputblocksize/) { get; } | Получает размер входного блока. |
| abstract [OutputBlockSize](../../aspose.zip.crypto/sevenzipcipher/outputblocksize/) { get; } | Получает размер выходного блока. |

## Методы

| Имя | Описание |
| --- | --- |
| abstract [Dispose](../../aspose.zip.crypto/sevenzipcipher/dispose/)() | Выполняет определяемые приложением задачи, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| abstract [TransformBlock](../../aspose.zip.crypto/sevenzipcipher/transformblock/)(byte[], int, int, byte[], int) | Преобразует указанную область входного массива байтов и копирует результирующее преобразование в указанную область выходного массива байтов. |
| abstract [TransformFinalBlock](../../aspose.zip.crypto/sevenzipcipher/transformfinalblock/)(byte[], int, int) | Преобразует указанную область указанного массива байтов. |

### Смотрите также

* пространство имен [Aspose.Zip.Crypto](../../aspose.zip.crypto/)
* сборка [Aspose.Zip](../../)


