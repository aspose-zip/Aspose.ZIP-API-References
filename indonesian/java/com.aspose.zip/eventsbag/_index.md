---
title: "EventsBag"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Kontainer peristiwa yang digunakan saat menyimpan."
type: docs
weight: 65
url: /id/java/com.aspose.zip/eventsbag/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBag
```

Kontainer peristiwa yang digunakan saat menyimpan [Archive](../../com.aspose.zip/archive).
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [EventsBag()](#EventsBag--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Mendapatkan peristiwa yang dipicu sebelum entri arsip dikompresi. |
| [getEntryCompressed()](#getEntryCompressed--) | Mendapatkan peristiwa yang dipicu setelah entri arsip telah dikompresi. |
| [setEntryAccessed(Event&lt;EntryEventArgs&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | Mengatur peristiwa yang dipicu sebelum entri arsip dikompresi. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--) | Mengatur peristiwa yang dipicu setelah entri arsip telah dikompresi. |
### EventsBag() {#EventsBag--}
```
public EventsBag()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgs> getEntryAccessed()
```


Mendapatkan peristiwa yang dipicu sebelum entri arsip dikompresi.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgs> getEntryCompressed()
```


Mendapatkan peristiwa yang dipicu setelah entri arsip telah dikompresi.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgs&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public void setEntryAccessed(Event<EntryEventArgs> value)
```


Mengatur peristiwa yang dipicu sebelum entri arsip dikompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgs&gt; | sebuah peristiwa yang dipicu sebelum entri arsip dikompresi. |

### setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--}
```
public void setEntryCompressed(Event<CancelEntryEventArgs> value)
```


Mengatur peristiwa yang dipicu setelah entri arsip telah dikompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgs&gt; | sebuah peristiwa yang dipicu setelah entri arsip telah dikompresi |

