---
title: "EventsBagXar"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "حاوية الأحداث المستخدمة عند الحفظ."
type: docs
weight: 67
url: /ar/java/com.aspose.zip/eventsbagxar/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagXar
```

حاوية الأحداث المستخدمة عند حفظ [XarArchive](../../com.aspose.zip/xararchive).
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [EventsBagXar()](#EventsBagXar--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | يحصل على حدث يُرفع قبل ضغط مدخل الأرشيف. |
| [getEntryCompressed()](#getEntryCompressed--) | يحصل على حدث يُرفع بعد ضغط مدخل الأرشيف. |
| [setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--) | يضبط حدثًا يُرفع قبل ضغط مدخل الأرشيف. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--) | يضبط حدثًا يُرفع بعد ضغط مدخل الأرشيف. |
### EventsBagXar() {#EventsBagXar--}
```
public EventsBagXar()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsXar> getEntryAccessed()
```


يحصل على حدث يُرفع قبل ضغط مدخل الأرشيف.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgsXar> getEntryCompressed()
```


يحصل على حدث يُرفع بعد ضغط مدخل الأرشيف.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--}
```
public void setEntryAccessed(Event<EntryEventArgsXar> value)
```


يضبط حدثًا يُرفع قبل ضغط مدخل الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsXar&gt; | حدث يُرفع قبل ضغط مدخل الأرشيف. |

### setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--}
```
public void setEntryCompressed(Event<CancelEntryEventArgsXar> value)
```


يضبط حدثًا يُرفع بعد ضغط مدخل الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgsXar&gt; | حدث يُرفع بعد ضغط مدخل الأرشيف |

