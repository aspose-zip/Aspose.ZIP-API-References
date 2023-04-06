---
title: ArchiveLoadOptions.Encoding
second_title: Aspose.ZIP for .NET API 参考
description: ArchiveLoadOptions 财产. 获取或设置条目名称的编码
type: docs
weight: 30
url: /zh/net/aspose.zip/archiveloadoptions/encoding/
---
## ArchiveLoadOptions.Encoding property

获取或设置条目名称的编码。

```csharp
public Encoding Encoding { get; set; }
```

### 例子

无论 zip 文件属性如何，条目名称都使用指定的编码组成。

```csharp
using (FileStream fs = File.OpenRead("archive.zip"))
{      
    using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(932) }))
    {
        string name = archive.Entries[0].Name;
    }    
}
```

### 也可以看看

* class [ArchiveLoadOptions](../)
* 命名空间 [Aspose.Zip](../../archiveloadoptions/)
* 部件 [Aspose.Zip](../../../)


