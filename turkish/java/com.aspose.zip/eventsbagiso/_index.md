---
title: "EventsBagIso"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Kaydetme sırasında kullanılan olay kapsayıcısı."
type: docs
weight: 66
url: /tr/java/com.aspose.zip/eventsbagiso/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagIso
```

[IsoArchive](../../com.aspose.zip/isoarchive) kaydetme sırasında kullanılan olay konteyneri.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [EventsBagIso()](#EventsBagIso--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Bir arşiv girdisi sıkıştırılmadan önce tetiklenen bir olayı alır. |
| [getEntryCompressed()](#getEntryCompressed--) | Bir arşiv girdisi sıkıştırıldıktan sonra tetiklenen bir olayı alır. |
| [setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Bir arşiv girdisi sıkıştırılmadan önce tetiklenen bir olayı ayarlar. |
| [setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Bir arşiv girdisi sıkıştırıldıktan sonra tetiklenen bir olayı ayarlar. |
### EventsBagIso() {#EventsBagIso--}
```
public EventsBagIso()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsIso> getEntryAccessed()
```


Bir arşiv girdisi sıkıştırılmadan önce tetiklenen bir olayı alır.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<EntryEventArgsIso> getEntryCompressed()
```


Bir arşiv girdisi sıkıştırıldıktan sonra tetiklenen bir olayı alır.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryAccessed(Event<EntryEventArgsIso> value)
```


Bir arşiv girdisi sıkıştırılmadan önce tetiklenen bir olayı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | Bir arşiv girdisi sıkıştırılmadan önce tetiklenen bir olay. |

### setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryCompressed(Event<EntryEventArgsIso> value)
```


Bir arşiv girdisi sıkıştırıldıktan sonra tetiklenen bir olayı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | Bir arşiv girdisi sıkıştırıldıktan sonra tetiklenen bir olay |

