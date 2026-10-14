---
title: "FastLZStream.FastLZStream"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "FastLZStream コンストラクタ。圧縮用に準備された FastLZStream クラスの新しいインスタンスを初期化します"
type: docs
weight: 10
url: /ja/net/aspose.zip.fastlz/fastlzstream/fastlzstream/
---
## FastLZStream constructor

圧縮用に準備された [`FastLZStream`](../) クラスの新しいインスタンスを初期化します。

```csharp
public FastLZStream(Stream stream, int compressionLevel)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| stream | Stream | 圧縮データを保存するためのストリームです。 |
| compressionLevel | Int32 | 高速な圧縮のためには 1 を、より高い圧縮率のためには 2 を使用します。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *stream* は null です。 |
| ArgumentException | *stream* は書き込みをサポートしていません。 |
| ArgumentOutOfRangeException | *compressionLevel* は 2 より大きい、または 1 未満です。 |

### 関連項目

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


