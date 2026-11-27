---
title: "EventsBag"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "حاوية الأحداث المستخدمة عند الحفظ."
type: docs
weight: 65
url: /ar/java/com.aspose.zip/eventsbag/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBag
```

حاوية الأحداث المستخدمة عند حفظ [Archive](../../com.aspose.zip/archive).
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [EventsBag()](#EventsBag--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | يحصل على حدث يُرفع قبل ضغط مدخل الأرشيف. |
| [getEntryCompressed()](#getEntryCompressed--) | يحصل على حدث يُرفع بعد ضغط مدخل الأرشيف. |
| [setEntryAccessed(Event&lt;EntryEventArgs&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | يضبط حدثًا يُرفع قبل ضغط مدخل الأرشيف. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--) | يضبط حدثًا يُرفع بعد ضغط مدخل الأرشيف. |
### EventsBag() {#EventsBag--}
```
public EventsBag()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgs> getEntryAccessed()
```


يحصل على حدث يُرفع قبل ضغط مدخل الأرشيف.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgs> getEntryCompressed()
```


يحصل على حدث يُرفع بعد ضغط مدخل الأرشيف.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgs&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public void setEntryAccessed(Event<EntryEventArgs> value)
```


يضبط حدثًا يُرفع قبل ضغط مدخل الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgs&gt; | حدث يُرفع قبل ضغط مدخل الأرشيف. |

### setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--}
```
public void setEntryCompressed(Event<CancelEntryEventArgs> value)
```


يضبط حدثًا يُرفع بعد ضغط مدخل الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgs&gt; | حدث يُرفع بعد ضغط مدخل الأرشيف |

