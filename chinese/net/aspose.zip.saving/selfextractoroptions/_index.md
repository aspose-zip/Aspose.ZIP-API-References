---
title: Class SelfExtractorOptions
second_title: Aspose.ZIP for .NET API 参考
description: Aspose.Zip.Saving.SelfExtractorOptions 班级. 创建自解压可执行文件的选项
type: docs
weight: 500
url: /zh/net/aspose.zip.saving/selfextractoroptions/
---
## SelfExtractorOptions class

创建自解压可执行文件的选项。

```csharp
public class SelfExtractorOptions
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [SelfExtractorOptions](selfextractoroptions/)() | 默认构造函数。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [CloseWindowOnExtraction](../../aspose.zip.saving/selfextractoroptions/closewindowonextraction/) { get; set; } | 获取或设置一个值，该值指示提取器窗口是否必须在提取时关闭。 |
| [ExtractorTitle](../../aspose.zip.saving/selfextractoroptions/extractortitle/) { get; set; } | 获取或设置提取器窗口的标题。 |
| [RunAfterExtraction](../../aspose.zip.saving/selfextractoroptions/runafterextraction/) { get; set; } | 获取或设置压缩包解压完成后执行的程序。 |
| [TitleIcon](../../aspose.zip.saving/selfextractoroptions/titleicon/) { get; set; } | 获取或设置提取器应用程序主窗口标题图标的路径。 |

### 评论

自解压存档不能与计量许可证组成：[`MeteredLicense`](../../aspose.zip/meteredlicense/) .

### 例子

```csharp
using (FileStream zipFile = File.Open("archive.exe", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        var sfxOptions = new SelfExtractorOptions() { ExtractorTitle = "Extractor", CloseWindowOnExtraction = true, TitleIcon = "C:\pictorgam.ico" };
        archive.Save(zipFile, new ArchiveSaveOptions() { SelfExtractorOptions = sfxOptions });
    }
}
```

### 也可以看看

* 命名空间 [Aspose.Zip.Saving](../../aspose.zip.saving/)
* 部件 [Aspose.Zip](../../)


