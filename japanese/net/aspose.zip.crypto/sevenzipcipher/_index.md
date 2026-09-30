---
title: "クラス SevenZipCipher"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Crypto.SevenZipCipher クラス。7zip 暗号化に使用される AES 暗号の基底クラス"
type: docs
weight: 440
url: /ja/net/aspose.zip.crypto/sevenzipcipher/
---
## SevenZipCipher class

7-zip 暗号化に使用される AES 暗号の基底クラスです。

```csharp
public abstract class SevenZipCipher : ICryptoTransform
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| abstract [CanReuseTransform](../../aspose.zip.crypto/sevenzipcipher/canreusetransform/) { get; } | 現在の変換を再利用できるかどうかを示す値を取得します。 |
| abstract [CanTransformMultipleBlocks](../../aspose.zip.crypto/sevenzipcipher/cantransformmultipleblocks/) { get; } | 複数ブロックを変換できるかどうかを示す値を取得します。 |
| abstract [InputBlockSize](../../aspose.zip.crypto/sevenzipcipher/inputblocksize/) { get; } | 入力ブロックサイズを取得します。 |
| abstract [OutputBlockSize](../../aspose.zip.crypto/sevenzipcipher/outputblocksize/) { get; } | 出力ブロックサイズを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| abstract [Dispose](../../aspose.zip.crypto/sevenzipcipher/dispose/)() | アンマネージド リソースの解放、リリース、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| abstract [TransformBlock](../../aspose.zip.crypto/sevenzipcipher/transformblock/)(byte[], int, int, byte[], int) | 入力バイト配列の指定領域を変換し、結果の変換を出力バイト配列の指定領域にコピーします。 |
| abstract [TransformFinalBlock](../../aspose.zip.crypto/sevenzipcipher/transformfinalblock/)(byte[], int, int) | 指定されたバイト配列の指定領域を変換します。 |

### 関連項目

* namespace [Aspose.Zip.Crypto](../../aspose.zip.crypto/)
* assembly [Aspose.Zip](../../)


