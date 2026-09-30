---
title: "类 FastLZStream"
second_title: "Aspose.ZIP for .NET API 参考"
description: "Aspose.Zip.FastLZ.FastLZStream 类。一个使用 FastLZ 压缩数据的流包装器。实现装饰器模式"
type: docs
weight: 500
url: /zh/net/aspose.zip.fastlz/fastlzstream/
---
## FastLZStream class

一个使用 FastLZ 压缩数据的流包装器。实现装饰器模式。

```csharp
public class FastLZStream : Stream
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [FastLZStream](fastlzstream/)(Stream, int) | 初始化一个准备压缩的 `FastLZStream` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| override [CanRead](../../aspose.zip.fastlz/fastlzstream/canread/) { get; } | 获取一个值，指示当前流是否支持读取。 |
| override [CanSeek](../../aspose.zip.fastlz/fastlzstream/canseek/) { get; } | 获取一个值，指示当前流是否支持定位。 |
| override [CanWrite](../../aspose.zip.fastlz/fastlzstream/canwrite/) { get; } | 获取一个值，指示当前流是否支持写入。 |
| override [Length](../../aspose.zip.fastlz/fastlzstream/length/) { get; } | 获取流的字节长度。 |
| override [Position](../../aspose.zip.fastlz/fastlzstream/position/) { get; set; } | 获取或设置当前流中的位置。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [Close](../../aspose.zip.fastlz/fastlzstream/close/)() | 关闭当前流并释放与当前流关联的任何资源（如套接字和文件句柄）。 |
| override [Flush](../../aspose.zip.fastlz/fastlzstream/flush/)() | 清除此流的所有缓冲区，并导致任何缓冲的数据写入底层设备。 |
| override [Read](../../aspose.zip.fastlz/fastlzstream/read/)(byte[], int, int) | 从流中读取一系列字节，并将流中的位置前移读取的字节数。不支持。 |
| override [Seek](../../aspose.zip.fastlz/fastlzstream/seek/)(long, SeekOrigin) | 设置当前流中的位置。 |
| override [SetLength](../../aspose.zip.fastlz/fastlzstream/setlength/)(long) | 设置当前流的长度。 |
| override [Write](../../aspose.zip.fastlz/fastlzstream/write/)(byte[], int, int) | 将一系列字节写入压缩流，并将此流中的当前位置前移写入的字节数。 |

### 另请参阅

* namespace [Aspose.Zip.FastLZ](../../aspose.zip.fastlz/)
* assembly [Aspose.Zip](../../)


