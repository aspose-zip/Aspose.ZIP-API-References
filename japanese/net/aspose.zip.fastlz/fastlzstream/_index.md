---
title: "クラス FastLZStream"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.FastLZ.FastLZStream クラス。FastLZ でデータを圧縮するストリーム ラッパーです。デコレータ パターンを実装しています。"
type: docs
weight: 500
url: /ja/net/aspose.zip.fastlz/fastlzstream/
---
## FastLZStream class

FastLZ でデータを圧縮するストリームラッパーです。デコレーターパターンを実装しています。

```csharp
public class FastLZStream : Stream
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [FastLZStream](fastlzstream/)(Stream, int) | 圧縮用に準備された `FastLZStream` クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| override [CanRead](../../aspose.zip.fastlz/fastlzstream/canread/) { get; } | 現在のストリームが読み取りをサポートしているかどうかを示す値を取得します。 |
| override [CanSeek](../../aspose.zip.fastlz/fastlzstream/canseek/) { get; } | 現在のストリームがシークをサポートしているかどうかを示す値を取得します。 |
| override [CanWrite](../../aspose.zip.fastlz/fastlzstream/canwrite/) { get; } | 現在のストリームが書き込みをサポートしているかどうかを示す値を取得します。 |
| override [Length](../../aspose.zip.fastlz/fastlzstream/length/) { get; } | ストリームのバイト単位の長さを取得します。 |
| override [Position](../../aspose.zip.fastlz/fastlzstream/position/) { get; set; } | 現在のストリーム内の位置を取得または設定します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| override [Close](../../aspose.zip.fastlz/fastlzstream/close/)() | 現在のストリームを閉じ、現在のストリームに関連付けられたリソース（ソケットやファイルハンドルなど）を解放します。 |
| override [Flush](../../aspose.zip.fastlz/fastlzstream/flush/)() | このストリームのすべてのバッファをクリアし、バッファされたデータが基礎となるデバイスに書き込まれるようにします。 |
| override [Read](../../aspose.zip.fastlz/fastlzstream/read/)(byte[], int, int) | ストリームからバイトのシーケンスを読み取り、読み取ったバイト数だけストリーム内の位置を進めます。サポートされていません。 |
| override [Seek](../../aspose.zip.fastlz/fastlzstream/seek/)(long, SeekOrigin) | 現在のストリーム内の位置を設定します。 |
| override [SetLength](../../aspose.zip.fastlz/fastlzstream/setlength/)(long) | 現在のストリームの長さを設定します。 |
| override [Write](../../aspose.zip.fastlz/fastlzstream/write/)(byte[], int, int) | バイトのシーケンスを書き込み、圧縮ストリームに書き込み、そしてこのストリーム内の現在位置を書き込んだバイト数だけ進めます。 |

### 関連項目

* namespace [Aspose.Zip.FastLZ](../../aspose.zip.fastlz/)
* assembly [Aspose.Zip](../../)


