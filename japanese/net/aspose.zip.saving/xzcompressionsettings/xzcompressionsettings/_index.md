---
title: "XzCompressionSettings.XzCompressionSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "XzCompressionSettings コンストラクタ。XzCompressionSettings クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/xzcompressionsettings/xzcompressionsettings/
---
## XzCompressionSettings constructor

[`XzCompressionSettings`](../) クラスの新しいインスタンスを初期化します。

```csharp
public XzCompressionSettings()
```

## 例

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 関連項目

* class [XzCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../xzcompressionsettings/)
* assembly [Aspose.Zip](../../../)


