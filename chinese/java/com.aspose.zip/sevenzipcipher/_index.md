---
title: "SevenZipCipher"
second_title: "Aspose.ZIP for Java API 参考"
description: "用于 7-zip 加密的 AES 密码的基类。"
type: docs
weight: 110
url: /zh/java/com.aspose.zip/sevenzipcipher/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Security.Cryptography.ICryptoTransform
```
public abstract class SevenZipCipher implements System.Security.Cryptography.ICryptoTransform
```

用于 7-zip 加密的 AES 密码的基类。
## 方法

| 方法 | 描述 |
| --- | --- |
| [canReuseTransform()](#canReuseTransform--) | 获取一个值，指示当前转换是否可以重用。 |
| [canTransformMultipleBlocks()](#canTransformMultipleBlocks--) | 获取一个值，指示是否可以转换多个块。 |
| [dispose()](#dispose--) | 执行应用程序定义的任务，以释放、释放或重置非托管资源。 |
| [getInputBlockSize()](#getInputBlockSize--) | 获取输入块大小。 |
| [getOutputBlockSize()](#getOutputBlockSize--) | 获取输出块大小。 |
| [transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)](#transformBlock-byte---int-int-byte---int-) | 转换输入字节数组的指定区域，并将结果转换复制到输出字节数组的指定区域。 |
| [transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)](#transformFinalBlock-byte---int-int-) | 转换指定字节数组的指定区域。 |
### canReuseTransform() {#canReuseTransform--}
```
public abstract boolean canReuseTransform()
```


获取一个值，指示当前转换是否可以重用。

**Returns:**
boolean - 指示当前转换是否可以重用的值
### canTransformMultipleBlocks() {#canTransformMultipleBlocks--}
```
public abstract boolean canTransformMultipleBlocks()
```


获取一个值，指示是否可以转换多个块。

**Returns:**
boolean - 指示是否可以转换多个块的值
### dispose() {#dispose--}
```
public abstract void dispose()
```


执行应用程序定义的任务，以释放、释放或重置非托管资源。

### getInputBlockSize() {#getInputBlockSize--}
```
public abstract int getInputBlockSize()
```


获取输入块大小。

**Returns:**
int - 输入块大小
### getOutputBlockSize() {#getOutputBlockSize--}
```
public abstract int getOutputBlockSize()
```


获取输出块大小。

**Returns:**
int - 输出块大小
### transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset) {#transformBlock-byte---int-int-byte---int-}
```
public abstract int transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)
```


转换输入字节数组的指定区域，并将结果转换复制到输出字节数组的指定区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| inputBuffer | byte[] | 用于计算转换的输入 |
| inputOffset | int | 输入字节数组中开始使用数据的偏移量 |
| inputCount | int | 输入字节数组中用作数据的字节数 |
| outputBuffer | byte[] | 写入转换的输出 |
| outputOffset | int | 输出字节数组中开始写入数据的偏移量 |

**Returns:**
int - 已写入的字节数
### transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount) {#transformFinalBlock-byte---int-int-}
```
public abstract byte[] transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)
```


转换指定字节数组的指定区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| inputBuffer | byte[] | 用于计算转换的输入 |
| inputOffset | int | 输入字节数组中开始使用数据的偏移量 |
| inputCount | int | 输入字节数组中用作数据的字节数 |

**Returns:**
byte[] - 计算得到的转换
