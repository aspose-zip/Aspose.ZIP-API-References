---
title: "CancelEntryEventArgsXar"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "キャンセル可能なエントリ関連イベントのためのイベント引数。"
type: docs
weight: 53
url: /ja/java/com.aspose.zip/cancelentryeventargsxar/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgsXar](../../com.aspose.zip/entryeventargsxar)
```
public class CancelEntryEventArgsXar extends EntryEventArgsXar
```

キャンセル可能なエントリ関連イベントのためのイベント引数。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [CancelEntryEventArgsXar(XarEntry entry)](#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-) | 新しい [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getCancel()](#getCancel--) | イベントをキャンセルすべきかどうかを示す値を取得します。 |
| [setCancel(boolean value)](#setCancel-boolean-) | イベントをキャンセルすべきかどうかを示す値を設定します。 |
### CancelEntryEventArgsXar(XarEntry entry) {#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-}
```
public CancelEntryEventArgsXar(XarEntry entry)
```


新しい [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | アーカイブエントリがイベントの対象として発生します |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


イベントをキャンセルすべきかどうかを示す値を取得します。

**Returns:**
boolean - イベントをキャンセルすべき場合は true、そうでない場合は false
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


イベントをキャンセルすべきかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | イベントをキャンセルすべき場合は true、そうでない場合は false |

