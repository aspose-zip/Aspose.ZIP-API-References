---
title: "EntryEventArgs"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "エントリ関連イベントのためのイベント引数。"
type: docs
weight: 62
url: /ja/java/com.aspose.zip/entryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgs extends System.EventArgs
```

エントリ関連イベントのためのイベント引数。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [EntryEventArgs(ArchiveEntry entry)](#EntryEventArgs-com.aspose.zip.ArchiveEntry-) | 新しい [EntryEventArgs](../../com.aspose.zip/entryeventargs) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getEntry()](#getEntry--) | イベントが発生するアーカイブエントリを取得します。 |
### EntryEventArgs(ArchiveEntry entry) {#EntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public EntryEventArgs(ArchiveEntry entry)
```


新しい [EntryEventArgs](../../com.aspose.zip/entryeventargs) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | イベントが発生する対象のアーカイブエントリ。 |

### getEntry() {#getEntry--}
```
public final ArchiveEntry getEntry()
```


イベントが発生するアーカイブエントリを取得します。

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - the archive entry the event is raised for.
