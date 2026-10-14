---
title: "LzmaArchiveSettings.DictionarySize"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "LzmaArchiveSettings プロパティ。辞書履歴バッファサイズは、最近処理された非圧縮データがメモリに保持されるバイト数を示します。設定されていない場合は、エントリサイズに応じて自動的に選択されます"
type: docs
weight: 20
url: /ja/net/aspose.zip.lzma/lzmaarchivesettings/dictionarysize/
---
## LzmaArchiveSettings.DictionarySize property

辞書（履歴バッファ）のサイズは、最近処理された非圧縮データがメモリに保持されるバイト数を示します。設定されていない場合、エントリサイズに応じて自動的に選択されます。

```csharp
public int DictionarySize { get; set; }
```

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentOutOfRangeException | 値が小さすぎるか大きすぎます。 |
| ArgumentException | 値が 2 のべき乗でも 2 のべき乗の 3 倍でもありません。 |

## 備考

辞書が大きいほど、通常は圧縮率が向上しますが、非圧縮データよりも大きな辞書は RAM の無駄になります。

LZMA アーカイブの辞書サイズは、2 のべき乗 (2^n) または 2 のべき乗の 3 倍 (3*2^n) のいずれかでなければなりません。

### 関連項目

* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


