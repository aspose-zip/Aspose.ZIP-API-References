---
title: LzmaArchiveSettings.LzmaArchiveSettings
second_title: Aspose.ZIP for .NET API リファレンス
description: LzmaArchiveSettings コンストラクタ. の新しいインスタンスを初期化しますLzmaArchiveSettingsデフォルトのディクショナリ サイズを持つクラスで16 メガバイトに相当します
type: docs
weight: 10
url: /ja/net/aspose.zip.lzma/lzmaarchivesettings/lzmaarchivesettings/
---
## LzmaArchiveSettings constructor

の新しいインスタンスを初期化します[`LzmaArchiveSettings`](../)デフォルトのディクショナリ サイズを持つクラスで、16 メガバイトに相当します。

```csharp
public LzmaArchiveSettings()
```

### 例

```csharp
using (LzmaArchive archive = new LzmaArchive(new LzmaArchiveSettings() { DictionarySize = 1048576 } )
{
    archive.SetSource("data.bin);
    archive.Save(lzmaFile);
}
```

### 関連項目

* class [LzmaArchiveSettings](../)
* 名前空間 [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* 組み立て [Aspose.Zip](../../../)


