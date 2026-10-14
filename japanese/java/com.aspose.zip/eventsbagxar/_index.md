---
title: "EventsBagXar"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "保存時に使用されるイベントコンテナです。"
type: docs
weight: 67
url: /ja/java/com.aspose.zip/eventsbagxar/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagXar
```

保存時に使用されるイベントコンテナです。[XarArchive](../../com.aspose.zip/xararchive) の保存。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [EventsBagXar()](#EventsBagXar--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | アーカイブエントリが圧縮される前に発生するイベントを取得します。 |
| [getEntryCompressed()](#getEntryCompressed--) | アーカイブエントリが圧縮された後に発生するイベントを取得します。 |
| [setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--) | アーカイブエントリが圧縮される前に発生するイベントを設定します。 |
| [setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--) | アーカイブエントリが圧縮された後に発生するイベントを設定します。 |
### EventsBagXar() {#EventsBagXar--}
```
public EventsBagXar()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsXar> getEntryAccessed()
```


アーカイブエントリが圧縮される前に発生するイベントを取得します。

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgsXar> getEntryCompressed()
```


アーカイブエントリが圧縮された後に発生するイベントを取得します。

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--}
```
public void setEntryAccessed(Event<EntryEventArgsXar> value)
```


アーカイブエントリが圧縮される前に発生するイベントを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsXar&gt; | アーカイブエントリが圧縮される前に発生するイベント。 |

### setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--}
```
public void setEntryCompressed(Event<CancelEntryEventArgsXar> value)
```


アーカイブエントリが圧縮された後に発生するイベントを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgsXar&gt; | アーカイブエントリが圧縮された後に発生するイベント |

