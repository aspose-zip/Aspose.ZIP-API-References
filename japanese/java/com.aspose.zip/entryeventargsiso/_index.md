---
title: "EntryEventArgsIso"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "エントリ関連イベントのためのイベント引数。"
type: docs
weight: 63
url: /ja/java/com.aspose.zip/entryeventargsiso/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgsIso extends System.EventArgs
```

エントリ関連イベントのためのイベント引数。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [EntryEventArgsIso(IsoEntry entry)](#EntryEventArgsIso-com.aspose.zip.IsoEntry-) | 新しい [EntryEventArgs](../../com.aspose.zip/entryeventargs) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getEntry()](#getEntry--) | イベントが発生するアーカイブエントリを取得します。 |
### EntryEventArgsIso(IsoEntry entry) {#EntryEventArgsIso-com.aspose.zip.IsoEntry-}
```
public EntryEventArgsIso(IsoEntry entry)
```


新しい [EntryEventArgs](../../com.aspose.zip/entryeventargs) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| entry | [IsoEntry](../../com.aspose.zip/isoentry) | イベントが発生するアーカイブエントリ |

### getEntry() {#getEntry--}
```
public final IsoEntry getEntry()
```


イベントが発生するアーカイブエントリを取得します。

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the archive entry the event is raised for
