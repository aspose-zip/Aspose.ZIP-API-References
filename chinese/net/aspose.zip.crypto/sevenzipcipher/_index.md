---
title: Class SevenZipCipher
second_title: Aspose.ZIP for .NET API 参考
description: Aspose.Zip.Crypto.SevenZipCipher 班级. 用于 7zip 加密的 AES 密码的基类
type: docs
weight: 190
url: /zh/net/aspose.zip.crypto/sevenzipcipher/
---
## SevenZipCipher class

用于 7-zip 加密的 AES 密码的基类。

```csharp
public abstract class SevenZipCipher : ICryptoTransform
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| abstract [CanReuseTransform](../../aspose.zip.crypto/sevenzipcipher/canreusetransform/) { get; } | 获取一个值，指示当前转换是否可以重复使用。 |
| abstract [CanTransformMultipleBlocks](../../aspose.zip.crypto/sevenzipcipher/cantransformmultipleblocks/) { get; } | 获取一个值，表示是否可以转换多个块。 |
| abstract [InputBlockSize](../../aspose.zip.crypto/sevenzipcipher/inputblocksize/) { get; } | 获取输入块大小。 |
| abstract [OutputBlockSize](../../aspose.zip.crypto/sevenzipcipher/outputblocksize/) { get; } | 获取输出块大小。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| abstract [Dispose](../../aspose.zip.crypto/sevenzipcipher/dispose/)() | 执行与释放、释放或重置非托管资源相关的应用程序定义的任务。 |
| abstract [TransformBlock](../../aspose.zip.crypto/sevenzipcipher/transformblock/)(byte[], int, int, byte[], int) | 转换输入字节数组的指定区域并将生成的转换复制到输出字节数组的指定区域。 |
| abstract [TransformFinalBlock](../../aspose.zip.crypto/sevenzipcipher/transformfinalblock/)(byte[], int, int) | 转换指定字节数组的指定区域。 |

### 也可以看看

* 命名空间 [Aspose.Zip.Crypto](../../aspose.zip.crypto/)
* 部件 [Aspose.Zip](../../)


