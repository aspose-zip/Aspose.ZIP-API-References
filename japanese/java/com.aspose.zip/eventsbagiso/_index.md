---
title: "EventsBagIso"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "保存時に使用されるイベントコンテナです。"
type: docs
weight: 66
url: /ja/java/com.aspose.zip/eventsbagiso/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagIso
```

[IsoArchive](../../com.aspose.zip/isoarchive) の保存時に使用されるイベントコンテナです。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [EventsBagIso()](#EventsBagIso--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | アーカイブエントリが圧縮される前に発生するイベントを取得します。 |
| [getEntryCompressed()](#getEntryCompressed--) | アーカイブエントリが圧縮された後に発生するイベントを取得します。 |
| [setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | アーカイブエントリが圧縮される前に発生するイベントを設定します。 |
| [setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | アーカイブエントリが圧縮された後に発生するイベントを設定します。 |
### EventsBagIso() {#EventsBagIso--}
```
public EventsBagIso()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsIso> getEntryAccessed()
```


アーカイブエントリが圧縮される前に発生するイベントを取得します。

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<EntryEventArgsIso> getEntryCompressed()
```


アーカイブエントリが圧縮された後に発生するイベントを取得します。

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryAccessed(Event<EntryEventArgsIso> value)
```


アーカイブエントリが圧縮される前に発生するイベントを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | アーカイブエントリが圧縮される前に発生するイベント。 |

### setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryCompressed(Event<EntryEventArgsIso> value)
```


アーカイブエントリが圧縮された後に発生するイベントを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | アーカイブエントリが圧縮された後に発生するイベント |

