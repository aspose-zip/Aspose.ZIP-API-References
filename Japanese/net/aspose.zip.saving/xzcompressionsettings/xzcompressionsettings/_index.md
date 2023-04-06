---
title: XzCompressionSettings.XzCompressionSettings
second_title: Aspose.ZIP for .NET API リファレンス
description: XzCompressionSettings コンストラクタ. の新しいインスタンスを初期化しますXzCompressionSettingsclass.
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/xzcompressionsettings/xzcompressionsettings/
---
## XzCompressionSettings constructor

の新しいインスタンスを初期化します[`XzCompressionSettings`](../)class.

```csharp
public XzCompressionSettings()
```

### 例

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 関連項目

* class [XzCompressionSettings](../)
* 名前空間 [Aspose.Zip.Saving](../../xzcompressionsettings/)
* 組み立て [Aspose.Zip](../../../)


