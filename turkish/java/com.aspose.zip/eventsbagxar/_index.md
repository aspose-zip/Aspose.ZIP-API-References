---
title: "EventsBagXar"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Kaydetme sırasında kullanılan olay kapsayıcısı."
type: docs
weight: 67
url: /tr/java/com.aspose.zip/eventsbagxar/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagXar
```

Kaydetme sırasında [XarArchive](../../com.aspose.zip/xararchive) kullanılan olay kapsayıcısı.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [EventsBagXar()](#EventsBagXar--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Bir arşiv girdisi sıkıştırılmadan önce tetiklenen bir olayı alır. |
| [getEntryCompressed()](#getEntryCompressed--) | Bir arşiv girdisi sıkıştırıldıktan sonra tetiklenen bir olayı alır. |
| [setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--) | Bir arşiv girdisi sıkıştırılmadan önce tetiklenen bir olayı ayarlar. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--) | Bir arşiv girdisi sıkıştırıldıktan sonra tetiklenen bir olayı ayarlar. |
### EventsBagXar() {#EventsBagXar--}
```
public EventsBagXar()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsXar> getEntryAccessed()
```


Bir arşiv girdisi sıkıştırılmadan önce tetiklenen bir olayı alır.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgsXar> getEntryCompressed()
```


Bir arşiv girdisi sıkıştırıldıktan sonra tetiklenen bir olayı alır.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--}
```
public void setEntryAccessed(Event<EntryEventArgsXar> value)
```


Bir arşiv girdisi sıkıştırılmadan önce tetiklenen bir olayı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsXar&gt; | Bir arşiv girdisi sıkıştırılmadan önce tetiklenen bir olay. |

### setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--}
```
public void setEntryCompressed(Event<CancelEntryEventArgsXar> value)
```


Bir arşiv girdisi sıkıştırıldıktan sonra tetiklenen bir olayı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgsXar&gt; | Bir arşiv girdisi sıkıştırıldıktan sonra tetiklenen bir olay |

