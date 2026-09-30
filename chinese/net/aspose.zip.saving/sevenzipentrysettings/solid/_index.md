---
title: "SevenZipEntrySettings.Solid"
second_title: "Aspose.ZIP for .NET API 参考"
description: "SevenZipEntrySettings 属性。获取或设置指示是否将条目连接并视为单个数据块的值"
type: docs
weight: 50
url: /zh/net/aspose.zip.saving/sevenzipentrysettings/solid/
---
## SevenZipEntrySettings.Solid property

获取或设置指示是否将条目连接并视为单个数据块的值。

```csharp
public bool Solid { get; set; }
```

## 备注

在创建存档时提供用于固态 7z 存档的 `SevenZipEntrySettings`。

## 示例

以下示例展示了如何在不加密的情况下使用 LZMA2 压缩将目录压缩为固态 7z 存档。

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings()){ Solid = true }))
    {
        archive.CreateEntries("C:\\Documents");
        archive.Save(sevenZipFile);
    }
}
```

### 另请参阅

* class [SevenZipEntrySettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipentrysettings/)
* assembly [Aspose.Zip](../../../)


