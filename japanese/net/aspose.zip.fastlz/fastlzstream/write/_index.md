---
title: "FastLZStream.Write"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "FastLZStream メソッド。バイトのシーケンスを書き込み、書き込まれたバイト数だけこのストリーム内の現在位置を進めます。"
type: docs
weight: 120
url: /ja/net/aspose.zip.fastlz/fastlzstream/write/
---
## FastLZStream.Write method

バイトのシーケンスを書き込み、圧縮ストリームに書き込み、そしてこのストリーム内の現在位置を書き込んだバイト数だけ進めます。

```csharp
public override void Write(byte[] buffer, int offset, int count)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| バッファ | Byte[] | バイトの配列。このメソッドは buffer から現在のストリームへ count バイトをコピーします。 |
| offset | Int32 | 現在のストリームへバイトのコピーを開始する buffer 内のゼロベースのバイトオフセット。 |
| count | Int32 | 現在のストリームに書き込まれるバイト数。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | ストリームが破棄されている場合にスローされます。 |
| ArgumentNullException | *buffer* は `null` です。 |

### 関連項目

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


