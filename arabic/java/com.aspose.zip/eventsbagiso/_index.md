---
title: "EventsBagIso"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "حاوية الأحداث المستخدمة عند الحفظ."
type: docs
weight: 66
url: /ar/java/com.aspose.zip/eventsbagiso/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagIso
```

حاوية الأحداث المستخدمة عند حفظ [IsoArchive](../../com.aspose.zip/isoarchive).
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [EventsBagIso()](#EventsBagIso--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | يحصل على حدث يُرفع قبل ضغط مدخل الأرشيف. |
| [getEntryCompressed()](#getEntryCompressed--) | يحصل على حدث يُرفع بعد ضغط مدخل الأرشيف. |
| [setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | يضبط حدثًا يُرفع قبل ضغط مدخل الأرشيف. |
| [setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | يضبط حدثًا يُرفع بعد ضغط مدخل الأرشيف. |
### EventsBagIso() {#EventsBagIso--}
```
public EventsBagIso()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsIso> getEntryAccessed()
```


يحصل على حدث يُرفع قبل ضغط مدخل الأرشيف.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<EntryEventArgsIso> getEntryCompressed()
```


يحصل على حدث يُرفع بعد ضغط مدخل الأرشيف.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryAccessed(Event<EntryEventArgsIso> value)
```


يضبط حدثًا يُرفع قبل ضغط مدخل الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | حدث يُرفع قبل ضغط مدخل الأرشيف. |

### setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryCompressed(Event<EntryEventArgsIso> value)
```


يضبط حدثًا يُرفع بعد ضغط مدخل الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | حدث يُرفع بعد ضغط مدخل الأرشيف |

