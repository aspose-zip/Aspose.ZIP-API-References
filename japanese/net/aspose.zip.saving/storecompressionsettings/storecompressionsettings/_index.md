---
title: "StoreCompressionSettings.StoreCompressionSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "StoreCompressionSettings コンストラクタ。StoreCompressionSettings クラスの新しいインスタンスを初期化します"
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/storecompressionsettings/storecompressionsettings/
---
## StoreCompressionSettings constructor

[`StoreCompressionSettings`](../) クラスの新しいインスタンスを初期化します。

```csharp
public StoreCompressionSettings()
```

## 例

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### 関連項目

* class [StoreCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../storecompressionsettings/)
* assembly [Aspose.Zip](../../../)


