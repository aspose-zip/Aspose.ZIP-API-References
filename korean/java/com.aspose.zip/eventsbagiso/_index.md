---
title: "EventsBagIso"
second_title: "Aspose.ZIP for Java API 참조"
description: "저장 시 사용되는 이벤트 컨테이너."
type: docs
weight: 66
url: /ko/java/com.aspose.zip/eventsbagiso/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagIso
```

[IsoArchive](../../com.aspose.zip/isoarchive) 저장에 사용되는 이벤트 컨테이너.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [EventsBagIso()](#EventsBagIso--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | 아카이브 항목이 압축되기 전에 발생하는 이벤트를 가져옵니다. |
| [getEntryCompressed()](#getEntryCompressed--) | 아카이브 항목이 압축된 후 발생하는 이벤트를 가져옵니다. |
| [setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | 아카이브 항목이 압축되기 전에 발생하는 이벤트를 설정합니다. |
| [setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | 아카이브 항목이 압축된 후 발생하는 이벤트를 설정합니다. |
### EventsBagIso() {#EventsBagIso--}
```
public EventsBagIso()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsIso> getEntryAccessed()
```


아카이브 항목이 압축되기 전에 발생하는 이벤트를 가져옵니다.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<EntryEventArgsIso> getEntryCompressed()
```


아카이브 항목이 압축된 후 발생하는 이벤트를 가져옵니다.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryAccessed(Event<EntryEventArgsIso> value)
```


아카이브 항목이 압축되기 전에 발생하는 이벤트를 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | 아카이브 항목이 압축되기 전에 발생하는 이벤트입니다. |

### setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryCompressed(Event<EntryEventArgsIso> value)
```


아카이브 항목이 압축된 후 발생하는 이벤트를 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | 아카이브 항목이 압축된 후에 발생하는 이벤트입니다 |

