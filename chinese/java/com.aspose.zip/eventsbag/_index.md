---
title: "EventsBag"
second_title: "Aspose.ZIP for Java API 参考"
description: "用于保存时的事件容器。"
type: docs
weight: 65
url: /zh/java/com.aspose.zip/eventsbag/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBag
```

Events container used on [Archive](../../com.aspose.zip/archive) saving.
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [EventsBag()](#EventsBag--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | 获取在压缩归档条目之前触发的事件。 |
| [getEntryCompressed()](#getEntryCompressed--) | 获取在归档条目压缩完成后触发的事件。 |
| [setEntryAccessed(Event&lt;EntryEventArgs&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | 设置在压缩归档条目之前触发的事件。 |
| [setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--) | 设置在归档条目压缩完成后触发的事件。 |
### EventsBag() {#EventsBag--}
```
public EventsBag()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgs> getEntryAccessed()
```


获取在压缩归档条目之前触发的事件。

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgs> getEntryCompressed()
```


获取在归档条目压缩完成后触发的事件。

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgs&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public void setEntryAccessed(Event<EntryEventArgs> value)
```


设置在压缩归档条目之前触发的事件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgs&gt; | 在归档条目被压缩之前触发的事件。 |

### setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--}
```
public void setEntryCompressed(Event<CancelEntryEventArgs> value)
```


设置在归档条目压缩完成后触发的事件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgs&gt; | 在归档条目被压缩之后触发的事件 |

