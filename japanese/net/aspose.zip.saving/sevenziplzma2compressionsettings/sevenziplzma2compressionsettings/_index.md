---
title: "SevenZipLZMA2CompressionSettings.SevenZipLZMA2CompressionSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SevenZipLZMA2CompressionSettings コンストラクタ。7z アーカイブ内の LZMA2 圧縮メソッドの設定をインスタンス化します"
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/sevenziplzma2compressionsettings/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings(int) {#constructor}

7z アーカイブ内の LZMA2 圧縮方式の設定をインスタンス化します。

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize = 16777216)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dictionarySize | Int32 | 履歴バッファのサイズは 4096 から 1073741824 の間である必要があります。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* が大きすぎるか小さすぎます。 |

## 備考

辞書が大きいほど、通常は圧縮率が向上しますが、非圧縮データよりも大きな辞書は RAM の無駄になります。

### 関連項目

* class [SevenZipLZMA2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipLZMA2CompressionSettings(int, int) {#constructor_1}

7z アーカイブ内の LZMA2 圧縮方式の設定をインスタンス化します。

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes = 32)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dictionarySize | Int32 | 履歴バッファのサイズは 4096 から 1073741824 の間である必要があります。 |
| fastBytes | Int32 | LZMA2 コンプレッサで使用される高速バイト数を制御します。高速バイト数を増やすと、圧縮速度を犠牲にして圧縮率を向上させることができます。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* が大きすぎるか小さすぎる、または *fastBytes* が大きすぎるか小さすぎる。 |

## 備考

辞書が大きいほど、通常は圧縮率が向上しますが、非圧縮データよりも大きな辞書は RAM の無駄になります。

### 関連項目

* class [SevenZipLZMA2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* assembly [Aspose.Zip](../../../)


