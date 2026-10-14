---
title: "LzipArchiveSettings.LzipArchiveSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "LzipArchiveSettings コンストラクタ。特定の辞書サイズで新しい LzipArchiveSettings のインスタンスを初期化します"
type: docs
weight: 10
url: /ja/net/aspose.zip.lzip/lziparchivesettings/lziparchivesettings/
---
## LzipArchiveSettings constructor

特定の辞書サイズで新しい [`LzipArchiveSettings`](../) のインスタンスを初期化します。

```csharp
public LzipArchiveSettings(int dictionarySize, int maxMemberSize = 62914560)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dictionarySize | Int32 | LZMA 圧縮用の辞書サイズ（バイト単位）。 |
| maxMemberSize | Int32 | lzip アーカイブ内の 1 メンバーあたりの最大サイズ（バイト単位）。デフォルト値は 60 MB です。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentOutOfRangeException | dictionarySize が許容範囲外の値である場合にスローされます。 |

### 関連項目

* class [LzipArchiveSettings](../)
* namespace [Aspose.Zip.Lzip](../../lziparchivesettings/)
* assembly [Aspose.Zip](../../../)


