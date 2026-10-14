---
title: "SevenZipCipher"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "7-zip 暗号化に使用される AES 暗号の基底クラス。"
type: docs
weight: 110
url: /ja/java/com.aspose.zip/sevenzipcipher/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Security.Cryptography.ICryptoTransform
```
public abstract class SevenZipCipher implements System.Security.Cryptography.ICryptoTransform
```

7-zip 暗号化に使用される AES 暗号の基底クラス。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [canReuseTransform()](#canReuseTransform--) | 現在の変換が再利用可能かどうかを示す値を取得します。 |
| [canTransformMultipleBlocks()](#canTransformMultipleBlocks--) | 複数のブロックを変換できるかどうかを示す値を取得します。 |
| [dispose()](#dispose--) | アンマネージ リソースの解放、リリース、またはリセットに関連するアプリケーション定義タスクを実行します。 |
| [getInputBlockSize()](#getInputBlockSize--) | 入力ブロックサイズを取得します。 |
| [getOutputBlockSize()](#getOutputBlockSize--) | 出力ブロックサイズを取得します。 |
| [transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)](#transformBlock-byte---int-int-byte---int-) | 入力バイト配列の指定領域を変換し、結果の変換を出力バイト配列の指定領域にコピーします。 |
| [transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)](#transformFinalBlock-byte---int-int-) | 指定されたバイト配列の指定領域を変換します。 |
### canReuseTransform() {#canReuseTransform--}
```
public abstract boolean canReuseTransform()
```


現在の変換が再利用可能かどうかを示す値を取得します。

**Returns:**
boolean - 現在の変換が再利用可能かどうかを示す値
### canTransformMultipleBlocks() {#canTransformMultipleBlocks--}
```
public abstract boolean canTransformMultipleBlocks()
```


複数のブロックを変換できるかどうかを示す値を取得します。

**Returns:**
boolean - 複数のブロックを変換できるかどうかを示す値
### dispose() {#dispose--}
```
public abstract void dispose()
```


アンマネージ リソースの解放、リリース、またはリセットに関連するアプリケーション定義タスクを実行します。

### getInputBlockSize() {#getInputBlockSize--}
```
public abstract int getInputBlockSize()
```


入力ブロックサイズを取得します。

**Returns:**
int - 入力ブロックのサイズ
### getOutputBlockSize() {#getOutputBlockSize--}
```
public abstract int getOutputBlockSize()
```


出力ブロックサイズを取得します。

**Returns:**
int - 出力ブロックのサイズ
### transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset) {#transformBlock-byte---int-int-byte---int-}
```
public abstract int transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)
```


入力バイト配列の指定領域を変換し、結果の変換を出力バイト配列の指定領域にコピーします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| inputBuffer | byte[] | 変換を計算する対象の入力 |
| inputOffset | int | データの使用を開始する入力バイト配列内のオフセット |
| inputCount | int | データとして使用する入力バイト配列内のバイト数 |
| outputBuffer | byte[] | 変換を書き込む出力 |
| outputOffset | int | データの書き込みを開始する出力バイト配列内のオフセット |

**Returns:**
int - 書き込まれたバイト数
### transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount) {#transformFinalBlock-byte---int-int-}
```
public abstract byte[] transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)
```


指定されたバイト配列の指定領域を変換します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| inputBuffer | byte[] | 変換を計算する対象の入力 |
| inputOffset | int | データの使用を開始する入力バイト配列内のオフセット |
| inputCount | int | データとして使用する入力バイト配列内のバイト数 |

**Returns:**
byte[] - 計算された変換
