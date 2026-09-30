---
title: "LzmaArchiveSettings.LzmaArchiveSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "LzmaArchiveSettings コンストラクタ。デフォルトの辞書サイズが 16 メガバイト、ファストバイト数が 32、リテラルコンテキストビットが 3 の LzmaArchiveSettings クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/aspose.zip.lzma/lzmaarchivesettings/lzmaarchivesettings/
---
## LzmaArchiveSettings constructor

デフォルトの辞書サイズが 16 メガバイト、ファストバイト数が 32、リテラルコンテキストビットが 3 の [`LzmaArchiveSettings`](../) クラスの新しいインスタンスを初期化します。

```csharp
public LzmaArchiveSettings()
```

## 例

```csharp
using (LzmaArchive archive = new LzmaArchive(new LzmaArchiveSettings() { DictionarySize = 1048576 })
{
    archive.SetSource("data.bin");
    archive.Save(lzmaFile);
}
```

### 関連項目

* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


