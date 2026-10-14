---
title: "SevenZipLZMACompressionSettings.DictionarySize"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SevenZipLZMACompressionSettings プロパティ。辞書履歴バッファサイズは、最近処理された非圧縮データの何バイトがメモリに保持されるかを示します。設定されていない場合はエントリサイズに応じて自動的に選択されます。4096 から 1073741824 の間である必要があり、エントリサイズに基づく自動検出のために 0 に設定することもできます。"
type: docs
weight: 20
url: /ja/net/aspose.zip.saving/sevenziplzmacompressionsettings/dictionarysize/
---
## SevenZipLZMACompressionSettings.DictionarySize property

辞書（履歴バッファ）サイズは、最近処理された非圧縮データがメモリに保持されるバイト数を示します。設定されていない場合、エントリサイズに応じて自動的に選択されます。サイズは 4096 から 1073741824 の間である必要があり、エントリサイズに基づく自動検出の場合は 0 を指定できます。

```csharp
public int DictionarySize { get; set; }
```

## 備考

辞書が大きいほど、通常は圧縮率が向上しますが、非圧縮データよりも大きな辞書は RAM の無駄になります。

### 関連項目

* class [SevenZipLZMACompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)


