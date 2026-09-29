---
title: "EventsBagXar"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Kontainer peristiwa yang digunakan saat menyimpan."
type: docs
weight: 67
url: /id/java/com.aspose.zip/eventsbagxar/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagXar
```

Kontainer peristiwa yang digunakan saat menyimpan [XarArchive](../../com.aspose.zip/xararchive).
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [EventsBagXar()](#EventsBagXar--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Mendapatkan peristiwa yang dipicu sebelum entri arsip dikompresi. |
| [getEntryCompressed()](#getEntryCompressed--) | Mendapatkan peristiwa yang dipicu setelah entri arsip telah dikompresi. |
| [setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--) | Mengatur peristiwa yang dipicu sebelum entri arsip dikompresi. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--) | Mengatur peristiwa yang dipicu setelah entri arsip telah dikompresi. |
### EventsBagXar() {#EventsBagXar--}
```
public EventsBagXar()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsXar> getEntryAccessed()
```


Mendapatkan peristiwa yang dipicu sebelum entri arsip dikompresi.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgsXar> getEntryCompressed()
```


Mendapatkan peristiwa yang dipicu setelah entri arsip telah dikompresi.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--}
```
public void setEntryAccessed(Event<EntryEventArgsXar> value)
```


Mengatur peristiwa yang dipicu sebelum entri arsip dikompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsXar&gt; | sebuah peristiwa yang dipicu sebelum entri arsip dikompresi. |

### setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--}
```
public void setEntryCompressed(Event<CancelEntryEventArgsXar> value)
```


Mengatur peristiwa yang dipicu setelah entri arsip telah dikompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgsXar&gt; | sebuah peristiwa yang dipicu setelah entri arsip telah dikompresi |

