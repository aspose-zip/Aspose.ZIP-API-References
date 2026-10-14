---
title: "CancelEntryEventArgs"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "キャンセル可能なエントリ関連イベントのためのイベント引数。"
type: docs
weight: 52
url: /ja/java/com.aspose.zip/cancelentryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgs](../../com.aspose.zip/entryeventargs)
```
public class CancelEntryEventArgs extends EntryEventArgs
```

キャンセル可能なエントリ関連イベントのためのイベント引数。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [CancelEntryEventArgs(ArchiveEntry entry)](#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-) | 新しい [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getCancel()](#getCancel--) | イベントをキャンセルすべきかどうかを示す値を取得します。 |
| [setCancel(boolean value)](#setCancel-boolean-) | イベントをキャンセルすべきかどうかを示す値を設定します。 |
### CancelEntryEventArgs(ArchiveEntry entry) {#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public CancelEntryEventArgs(ArchiveEntry entry)
```


新しい [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | イベントが発生する対象のアーカイブエントリ。 |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


イベントをキャンセルすべきかどうかを示す値を取得します。

**Returns:**
boolean - イベントをキャンセルすべき場合は true、そうでない場合は false。
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


イベントをキャンセルすべきかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | イベントをキャンセルすべき場合は true、そうでない場合は false。 |

