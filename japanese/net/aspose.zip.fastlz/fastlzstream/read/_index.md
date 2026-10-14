---
title: "FastLZStream.Read"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "FastLZStream メソッド。ストリームからバイトのシーケンスを読み取り、読み取ったバイト数だけストリーム内の位置を進めます。サポートされていません"
type: docs
weight: 90
url: /ja/net/aspose.zip.fastlz/fastlzstream/read/
---
## FastLZStream.Read method

ストリームからバイトのシーケンスを読み取り、読み取ったバイト数だけストリーム内の位置を進めます。サポートされていません。

```csharp
public override int Read(byte[] buffer, int offset, int count)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| バッファ | Byte[] | バイト配列。 このメソッドが戻ると、バッファには指定されたバイト配列が格納され、offset から (offset + count - 1) までの値は現在のソースから読み取られたバイトで置き換えられます。 |
| offset | Int32 | 現在のストリームから読み取ったデータの格納を開始するバッファ内のゼロベースのバイトオフセットです。 |
| count | Int32 | 現在のストリームから読み取る最大バイト数です。 |

### 戻り値

バッファに読み込まれたバイトの総数です。要求されたバイト数より少ない場合があります（そのバイト数が現在利用できない場合）、またはストリームの終端に達した場合はゼロ (0) になります。

### 例外

| 例外 | 条件 |
| --- | --- |
| NotSupportedException | この操作はサポートされていません。 |

### 関連項目

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


