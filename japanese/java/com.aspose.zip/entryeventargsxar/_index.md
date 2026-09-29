---
title: "EntryEventArgsXar"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "エントリ関連イベントのためのイベント引数。"
type: docs
weight: 64
url: /ja/java/com.aspose.zip/entryeventargsxar/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgsXar extends System.EventArgs
```

エントリ関連イベントのためのイベント引数。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [EntryEventArgsXar(XarEntry entry)](#EntryEventArgsXar-com.aspose.zip.XarEntry-) | 新しい [EntryEventArgs](../../com.aspose.zip/entryeventargs) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getEntry()](#getEntry--) | イベントが発生するアーカイブエントリを取得します。 |
### EntryEventArgsXar(XarEntry entry) {#EntryEventArgsXar-com.aspose.zip.XarEntry-}
```
public EntryEventArgsXar(XarEntry entry)
```


新しい [EntryEventArgs](../../com.aspose.zip/entryeventargs) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | イベントが発生するアーカイブエントリ |

### getEntry() {#getEntry--}
```
public final XarEntry getEntry()
```


イベントが発生するアーカイブエントリを取得します。

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - the archive entry the event is raised for
