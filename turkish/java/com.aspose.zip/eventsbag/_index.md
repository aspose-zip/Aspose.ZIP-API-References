---
title: "EventsBag"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Kaydetme sırasında kullanılan olay kapsayıcısı."
type: docs
weight: 65
url: /tr/java/com.aspose.zip/eventsbag/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBag
```

[Archive](../../com.aspose.zip/archive) kaydetme sırasında kullanılan olay kapsayıcısı.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [EventsBag()](#EventsBag--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Bir arşiv girdisi sıkıştırılmadan önce tetiklenen bir olayı alır. |
| [getEntryCompressed()](#getEntryCompressed--) | Bir arşiv girdisi sıkıştırıldıktan sonra tetiklenen bir olayı alır. |
| [setEntryAccessed(Event&lt;EntryEventArgs&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | Bir arşiv girdisi sıkıştırılmadan önce tetiklenen bir olayı ayarlar. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--) | Bir arşiv girdisi sıkıştırıldıktan sonra tetiklenen bir olayı ayarlar. |
### EventsBag() {#EventsBag--}
```
public EventsBag()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgs> getEntryAccessed()
```


Bir arşiv girdisi sıkıştırılmadan önce tetiklenen bir olayı alır.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgs> getEntryCompressed()
```


Bir arşiv girdisi sıkıştırıldıktan sonra tetiklenen bir olayı alır.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgs&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public void setEntryAccessed(Event<EntryEventArgs> value)
```


Bir arşiv girdisi sıkıştırılmadan önce tetiklenen bir olayı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgs&gt; | Bir arşiv girdisi sıkıştırılmadan önce tetiklenen bir olay. |

### setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--}
```
public void setEntryCompressed(Event<CancelEntryEventArgs> value)
```


Bir arşiv girdisi sıkıştırıldıktan sonra tetiklenen bir olayı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgs&gt; | Bir arşiv girdisi sıkıştırıldıktan sonra tetiklenen bir olay |

