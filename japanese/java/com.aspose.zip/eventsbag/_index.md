---
title: "EventsBag"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "保存時に使用されるイベントコンテナです。"
type: docs
weight: 65
url: /ja/java/com.aspose.zip/eventsbag/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBag
```

アーカイブの保存時に使用されるイベントコンテナです。[Archive](../../com.aspose.zip/archive)
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [EventsBag()](#EventsBag--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | アーカイブエントリが圧縮される前に発生するイベントを取得します。 |
| [getEntryCompressed()](#getEntryCompressed--) | アーカイブエントリが圧縮された後に発生するイベントを取得します。 |
| [setEntryAccessed(Event&lt;EntryEventArgs&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | アーカイブエントリが圧縮される前に発生するイベントを設定します。 |
| [setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--) | アーカイブエントリが圧縮された後に発生するイベントを設定します。 |
### EventsBag() {#EventsBag--}
```
public EventsBag()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgs> getEntryAccessed()
```


アーカイブエントリが圧縮される前に発生するイベントを取得します。

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgs> getEntryCompressed()
```


アーカイブエントリが圧縮された後に発生するイベントを取得します。

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgs&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public void setEntryAccessed(Event<EntryEventArgs> value)
```


アーカイブエントリが圧縮される前に発生するイベントを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgs&gt; | アーカイブエントリが圧縮される前に発生するイベント。 |

### setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--}
```
public void setEntryCompressed(Event<CancelEntryEventArgs> value)
```


アーカイブエントリが圧縮された後に発生するイベントを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgs&gt; | アーカイブエントリが圧縮された後に発生するイベント |

