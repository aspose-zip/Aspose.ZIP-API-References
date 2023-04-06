---
title: DeflateCompressionSettings.DeflateCompressionSettings
second_title: Aspose.ZIP for .NET API リファレンス
description: DeflateCompressionSettings コンストラクタ. の新しいインスタンスを初期化しますDeflateCompressionSettingsclass.
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/deflatecompressionsettings/deflatecompressionsettings/
---
## DeflateCompressionSettings constructor

の新しいインスタンスを初期化します[`DeflateCompressionSettings`](../)class.

```csharp
public DeflateCompressionSettings()
```

### 例

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### 関連項目

* class [DeflateCompressionSettings](../)
* 名前空間 [Aspose.Zip.Saving](../../deflatecompressionsettings/)
* 組み立て [Aspose.Zip](../../../)


