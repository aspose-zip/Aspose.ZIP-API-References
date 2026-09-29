---
title: "EventsBagXar"
second_title: "Aspose.ZIP for Java API 참조"
description: "저장 시 사용되는 이벤트 컨테이너."
type: docs
weight: 67
url: /ko/java/com.aspose.zip/eventsbagxar/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagXar
```

저장 시 [XarArchive](../../com.aspose.zip/xararchive) 에 사용되는 이벤트 컨테이너.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [EventsBagXar()](#EventsBagXar--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | 아카이브 항목이 압축되기 전에 발생하는 이벤트를 가져옵니다. |
| [getEntryCompressed()](#getEntryCompressed--) | 아카이브 항목이 압축된 후 발생하는 이벤트를 가져옵니다. |
| [setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--) | 아카이브 항목이 압축되기 전에 발생하는 이벤트를 설정합니다. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--) | 아카이브 항목이 압축된 후 발생하는 이벤트를 설정합니다. |
### EventsBagXar() {#EventsBagXar--}
```
public EventsBagXar()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsXar> getEntryAccessed()
```


아카이브 항목이 압축되기 전에 발생하는 이벤트를 가져옵니다.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgsXar> getEntryCompressed()
```


아카이브 항목이 압축된 후 발생하는 이벤트를 가져옵니다.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--}
```
public void setEntryAccessed(Event<EntryEventArgsXar> value)
```


아카이브 항목이 압축되기 전에 발생하는 이벤트를 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsXar&gt; | 아카이브 항목이 압축되기 전에 발생하는 이벤트입니다. |

### setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--}
```
public void setEntryCompressed(Event<CancelEntryEventArgsXar> value)
```


아카이브 항목이 압축된 후 발생하는 이벤트를 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgsXar&gt; | 아카이브 항목이 압축된 후에 발생하는 이벤트입니다 |

