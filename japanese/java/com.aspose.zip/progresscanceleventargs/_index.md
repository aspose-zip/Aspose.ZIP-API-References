---
title: "ProgressCancelEventArgs"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "処理されたバイト数を含むキャンセル可能なイベント データ用のクラス。"
type: docs
weight: 95
url: /ja/java/com.aspose.zip/progresscanceleventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.ProgressEventArgs](../../com.aspose.zip/progresseventargs)
```
public class ProgressCancelEventArgs extends ProgressEventArgs
```

処理されたバイト数を含むキャンセル可能なイベント データ用のクラス。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [ProgressCancelEventArgs(long proceededBytes)](#ProgressCancelEventArgs-long-) | 新しいインスタンスを初期化します。[ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs) クラス。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getCancel()](#getCancel--) | イベントをキャンセルすべきかどうかを示す値を取得します。 |
| [setCancel(boolean value)](#setCancel-boolean-) | イベントをキャンセルすべきかどうかを示す値を設定します。 |
### ProgressCancelEventArgs(long proceededBytes) {#ProgressCancelEventArgs-long-}
```
public ProgressCancelEventArgs(long proceededBytes)
```


新しいインスタンスを初期化します。[ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs) クラス。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| proceededBytes | long | 処理されたバイト数。 |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


イベントをキャンセルすべきかどうかを示す値を取得します。

**Returns:**
boolean - イベントをキャンセルすべき場合は true、そうでなければ false。
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


イベントをキャンセルすべきかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | イベントをキャンセルすべきかどうかを示す値。 |

