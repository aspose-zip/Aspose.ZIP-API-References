---
title: Class SevenZipCipher
second_title: Aspose.ZIP for .NET API リファレンス
description: Aspose.Zip.Crypto.SevenZipCipher クラス. 7zip 暗号化に使用される AES 暗号の基本クラス
type: docs
weight: 190
url: /ja/net/aspose.zip.crypto/sevenzipcipher/
---
## SevenZipCipher class

7-zip 暗号化に使用される AES 暗号の基本クラス。

```csharp
public abstract class SevenZipCipher : ICryptoTransform
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| abstract [CanReuseTransform](../../aspose.zip.crypto/sevenzipcipher/canreusetransform/) { get; } | 現在の変換を再利用できるかどうかを示す値を取得します. |
| abstract [CanTransformMultipleBlocks](../../aspose.zip.crypto/sevenzipcipher/cantransformmultipleblocks/) { get; } | 複数のブロックを変形できるかどうかを示す値を取得します。 |
| abstract [InputBlockSize](../../aspose.zip.crypto/sevenzipcipher/inputblocksize/) { get; } | 入力ブロックサイズを取得します. |
| abstract [OutputBlockSize](../../aspose.zip.crypto/sevenzipcipher/outputblocksize/) { get; } | 出力ブロックサイズを取得します. |

## メソッド

| 名前 | 説明 |
| --- | --- |
| abstract [Dispose](../../aspose.zip.crypto/sevenzipcipher/dispose/)() | アンマネージ リソースの解放、解放、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| abstract [TransformBlock](../../aspose.zip.crypto/sevenzipcipher/transformblock/)(byte[], int, int, byte[], int) | 入力バイト配列の指定された領域を変換し、結果の変換を出力バイト配列の指定された領域にコピーします。 |
| abstract [TransformFinalBlock](../../aspose.zip.crypto/sevenzipcipher/transformfinalblock/)(byte[], int, int) | 指定されたバイト配列の指定された領域を変換します。 |

### 関連項目

* 名前空間 [Aspose.Zip.Crypto](../../aspose.zip.crypto/)
* 組み立て [Aspose.Zip](../../)


