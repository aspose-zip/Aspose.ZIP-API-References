---
title: "FastLZOutputStream"
second_title: "Aspose.ZIP for Java API 参考"
description: "使用 FastLZ 压缩数据的流包装器。"
type: docs
weight: 68
url: /zh/java/com.aspose.zip/fastlzoutputstream/
---

**Inheritance:**
java.lang.Object, java.io.OutputStream
```
public class FastLZOutputStream extends OutputStream
```

一个使用 FastLZ 压缩数据的流包装器。实现装饰器模式。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [FastLZOutputStream(OutputStream stream, int compressionLevel)](#FastLZOutputStream-java.io.OutputStream-int-) | 初始化一个准备进行压缩的 FastLZStream 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [close()](#close--) | 关闭当前流并释放与当前流关联的任何资源（例如套接字和文件句柄）。 |
| [flush()](#flush--) | 清除此流的所有缓冲区，并导致任何缓冲的数据写入底层设备。 |
| [write(byte[] buffer, int offset, int count)](#write-byte---int-int-) | 将一系列字节写入压缩流，并根据写入的字节数推进此流中的当前位置。 |
| [write(int b)](#write-int-) | 将指定的字节写入此输出流。 |
### FastLZOutputStream(OutputStream stream, int compressionLevel) {#FastLZOutputStream-java.io.OutputStream-int-}
```
public FastLZOutputStream(OutputStream stream, int compressionLevel)
```


初始化一个准备进行压缩的 FastLZStream 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.OutputStream | 用于保存压缩数据的流 |
| compressionLevel | int | 使用 1 进行更快的压缩，使用 2 获得更好的压缩比 |

### close() {#close--}
```
public void close()
```


关闭当前流并释放与当前流关联的任何资源（例如套接字和文件句柄）。

### flush() {#flush--}
```
public void flush()
```


清除此流的所有缓冲区，并导致任何缓冲的数据写入底层设备。

### write(byte[] buffer, int offset, int count) {#write-byte---int-int-}
```
public void write(byte[] buffer, int offset, int count)
```


将一系列字节写入压缩流，并根据写入的字节数推进此流中的当前位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| buffer | byte[] | 字节数组。此方法将 count 字节从 buffer 复制到当前流 |
| offset | int | buffer 中的零基字节偏移量，指示从何处开始将字节复制到当前流 |
| count | int | 要写入当前流的字节数 |

### write(int b) {#write-int-}
```
public void write(int b)
```


将指定的字节写入此输出流。`write` 的通用约定是向输出流写入一个字节。要写入的字节是参数 `b` 的低八位。`b` 的高 24 位将被忽略。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| b | int | 该 `byte` |

