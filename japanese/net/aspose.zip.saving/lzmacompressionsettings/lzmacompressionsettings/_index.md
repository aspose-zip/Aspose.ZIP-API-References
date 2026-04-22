---
title: LzmaCompressionSettings.LzmaCompressionSettings
second_title: Aspose.ZIP for .NET API リファレンス
description: LzmaCompressionSettings コンストラクタ. の新しいインスタンスを初期化しますLzmaCompressionSettingsデフォルトのディクショナリ サイズを持つクラスで16 メガバイトに相当します
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/lzmacompressionsettings/lzmacompressionsettings/
---
## LzmaCompressionSettings constructor

の新しいインスタンスを初期化します[`LzmaCompressionSettings`](../)デフォルトのディクショナリ サイズを持つクラスで、16 メガバイトに相当します。

```csharp
public LzmaCompressionSettings()
```

### 例

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 関連項目

* class [LzmaCompressionSettings](../)
* 名前空間 [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* 組み立て [Aspose.Zip](../../../)


