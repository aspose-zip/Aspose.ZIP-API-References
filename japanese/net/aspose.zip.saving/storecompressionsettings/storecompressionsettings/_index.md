---
title: StoreCompressionSettings.StoreCompressionSettings
second_title: Aspose.ZIP for .NET API リファレンス
description: StoreCompressionSettings コンストラクタ. の新しいインスタンスを初期化しますStoreCompressionSettingsclass.
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/storecompressionsettings/storecompressionsettings/
---
## StoreCompressionSettings constructor

の新しいインスタンスを初期化します[`StoreCompressionSettings`](../)class.

```csharp
public StoreCompressionSettings()
```

### 例

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### 関連項目

* class [StoreCompressionSettings](../)
* 名前空間 [Aspose.Zip.Saving](../../storecompressionsettings/)
* 組み立て [Aspose.Zip](../../../)


