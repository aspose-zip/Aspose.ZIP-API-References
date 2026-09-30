---
title: "AlzArchiveLoadOptions.Encoding"
second_title: "Aspose.ZIP for .NET API 参考"
description: "AlzArchiveLoadOptions 属性。获取或设置条目名称的编码。默认是韩文 Windows 代码页 949 CP949。"
type: docs
weight: 40
url: /zh/net/aspose.zip.alz/alzarchiveloadoptions/encoding/
---
## AlzArchiveLoadOptions.Encoding property

获取或设置条目名称的编码。默认是韩文 Windows 代码页 949 (CP949)。

```csharp
public Encoding Encoding { get; set; }
```

## 备注

ALZ 存档历史上使用韩文 Windows ANSI 代码页来存储文件名。

## 示例

条目名称使用指定的编码组成。

```csharp
using (FileStream fs = File.OpenRead("archive.alz"))
{
    using (var archive = new AlzArchive(fs, new AlzArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(949) }))
    {
        string name = archive.Entries[0].Name;
    }
}
```

### 另请参阅

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


