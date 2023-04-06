---
title: SevenZipLZMA2CompressionSettings.SevenZipLZMA2CompressionSettings
second_title: Aspose.ZIP for .NET API リファレンス
description: SevenZipLZMA2CompressionSettings コンストラクタ. 7z アーカイブ内の LZMA2 圧縮方式の設定をインスタンス化します
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/sevenziplzma2compressionsettings/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings(int) {#constructor}

7z アーカイブ内の LZMA2 圧縮方式の設定をインスタンス化します。

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize = 16777216)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| dictionarySize | Int32 | 履歴バッファのサイズは、4096 から 1073741824 の間である必要があります。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize*大きすぎるか小さすぎます。 |

### 備考

通常、ディクショナリが大きいほど圧縮率は高くなりますが、圧縮されていないデータよりも大きなディクショナリは RAM を浪費します。

### 関連項目

* class [SevenZipLZMA2CompressionSettings](../)
* 名前空間 [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* 組み立て [Aspose.Zip](../../../)

---

## SevenZipLZMA2CompressionSettings(int, int) {#constructor_1}

7z アーカイブ内の LZMA2 圧縮方式の設定をインスタンス化します。

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes = 32)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| dictionarySize | Int32 | 履歴バッファのサイズは、4096 から 1073741824 の間である必要があります。 |
| fastBytes | Int32 | LZMA2 コンプレッサが使用する高速バイト数を制御します。高速バイト数が多いほど、圧縮速度は低下しますが、圧縮率は向上します。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize*大きすぎるか小さすぎる、または*fastBytes*大きすぎるか小さすぎます。 |

### 備考

通常、ディクショナリが大きいほど圧縮率は高くなりますが、圧縮されていないデータよりも大きなディクショナリは RAM を浪費します。

### 関連項目

* class [SevenZipLZMA2CompressionSettings](../)
* 名前空間 [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* 組み立て [Aspose.Zip](../../../)


