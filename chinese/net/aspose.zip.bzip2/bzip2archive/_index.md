---
title: Class Bzip2Archive
second_title: Aspose.ZIP for .NET API 参考
description: Aspose.Zip.Bzip2.Bzip2Archive 班级. 此类代表 bzip2 存档文件用它来编写或提取 bzip2 archives.
type: docs
weight: 100
url: /zh/net/aspose.zip.bzip2/bzip2archive/
---
## Bzip2Archive class

此类代表 bzip2 存档文件。用它来编写或提取 bzip2 archives.

```csharp
public class Bzip2Archive : IArchive, IArchiveFileEntry
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [Bzip2Archive](bzip2archive/#constructor)() | 初始化一个新的实例`Bzip2Archive`准备压缩的类. |
| [Bzip2Archive](bzip2archive/#constructor_1)(Stream) | 初始化一个新的实例`Bzip2Archive`准备解压的类. |
| [Bzip2Archive](bzip2archive/#constructor_2)(string) | 初始化一个新的实例`Bzip2Archive`准备解压的类. |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Dispose](../../aspose.zip.bzip2/bzip2archive/dispose/)() | 执行与释放、释放或重置非托管资源相关的应用程序定义的任务。 |
| [Extract](../../aspose.zip.bzip2/bzip2archive/extract/)(Stream) | 将存档提取到提供的流中。 |
| [Open](../../aspose.zip.bzip2/bzip2archive/open/)() | 打开存档进行提取并提供包含存档内容的流。 |
| [Save](../../aspose.zip.bzip2/bzip2archive/save/#save)(Stream, Bzip2SaveOptions) | 将存档保存到提供的流中。 |
| [Save](../../aspose.zip.bzip2/bzip2archive/save/#save_1)(string, Bzip2SaveOptions) | 将存档保存到提供的目标文件。 |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_2)(FileInfo) | 设置要在存档中压缩的内容。 |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_3)(Stream) | 设置要在存档中压缩的内容。 |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_4)(string) | 设置要在存档中压缩的内容。 |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource)(CpioArchive, CpioFormat) | 设置要在存档中压缩的内容。 |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_1)(TarArchive, TarFormat) | 设置要在存档中压缩的内容。 |

### 评论

bzip2 使用 Burrows-Wheeler 块排序文本压缩算法和霍夫曼编码来压缩文件。查看更多：https://en.wikipedia.org/wiki/Bzip2

### 也可以看看

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* 命名空间 [Aspose.Zip.Bzip2](../../aspose.zip.bzip2/)
* 部件 [Aspose.Zip](../../)


