---
title: "Класс SevenZipCipher"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Crypto.SevenZipCipher. Базовый класс для AES‑шифра, используемого в шифровании 7zip"
type: docs
weight: 440
url: /ru/net/aspose.zip.crypto/sevenzipcipher/
---
## SevenZipCipher class

Базовый класс для шифра AES, используемого для шифрования 7-zip.

```csharp
public abstract class SevenZipCipher : ICryptoTransform
```

## Свойства

| Имя | Описание |
| --- | --- |
| abstract [CanReuseTransform](../../aspose.zip.crypto/sevenzipcipher/canreusetransform/) { get; } | Возвращает значение, указывающее, может ли текущая трансформация быть переиспользована. |
| abstract [CanTransformMultipleBlocks](../../aspose.zip.crypto/sevenzipcipher/cantransformmultipleblocks/) { get; } | Возвращает значение, указывающее, могут ли быть преобразованы несколько блоков. |
| abstract [InputBlockSize](../../aspose.zip.crypto/sevenzipcipher/inputblocksize/) { get; } | Возвращает размер входного блока. |
| abstract [OutputBlockSize](../../aspose.zip.crypto/sevenzipcipher/outputblocksize/) { get; } | Возвращает размер выходного блока. |

## Методы

| Имя | Описание |
| --- | --- |
| abstract [Dispose](../../aspose.zip.crypto/sevenzipcipher/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| abstract [TransformBlock](../../aspose.zip.crypto/sevenzipcipher/transformblock/)(byte[], int, int, byte[], int) | Преобразует указанную область входного массива байтов и копирует полученную трансформацию в указанную область выходного массива байтов. |
| abstract [TransformFinalBlock](../../aspose.zip.crypto/sevenzipcipher/transformfinalblock/)(byte[], int, int) | Преобразует указанную область указанного массива байтов. |

### См. также

* namespace [Aspose.Zip.Crypto](../../aspose.zip.crypto/)
* assembly [Aspose.Zip](../../)


