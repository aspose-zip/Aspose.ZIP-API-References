---
title: "DeflateCompressionSettings.DeflateCompressionSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "DeflateCompressionSettings コンストラクタ。DeflateCompressionSettings クラスの新しいインスタンスを初期化します"
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/deflatecompressionsettings/deflatecompressionsettings/
---
## DeflateCompressionSettings constructor

[`DeflateCompressionSettings`](../) クラスの新しいインスタンスを初期化します。

```csharp
public DeflateCompressionSettings()
```

## 例

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### 関連項目

* class [DeflateCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../deflatecompressionsettings/)
* assembly [Aspose.Zip](../../../)


