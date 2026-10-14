---
title: "EventsBagIso"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Kontainer peristiwa yang digunakan saat menyimpan."
type: docs
weight: 66
url: /id/java/com.aspose.zip/eventsbagiso/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagIso
```

Kontainer peristiwa yang digunakan pada penyimpanan [IsoArchive](../../com.aspose.zip/isoarchive).
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [EventsBagIso()](#EventsBagIso--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Mendapatkan peristiwa yang dipicu sebelum entri arsip dikompresi. |
| [getEntryCompressed()](#getEntryCompressed--) | Mendapatkan peristiwa yang dipicu setelah entri arsip telah dikompresi. |
| [setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Mengatur peristiwa yang dipicu sebelum entri arsip dikompresi. |
| [setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Mengatur peristiwa yang dipicu setelah entri arsip telah dikompresi. |
### EventsBagIso() {#EventsBagIso--}
```
public EventsBagIso()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsIso> getEntryAccessed()
```


Mendapatkan peristiwa yang dipicu sebelum entri arsip dikompresi.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<EntryEventArgsIso> getEntryCompressed()
```


Mendapatkan peristiwa yang dipicu setelah entri arsip telah dikompresi.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryAccessed(Event<EntryEventArgsIso> value)
```


Mengatur peristiwa yang dipicu sebelum entri arsip dikompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | sebuah peristiwa yang dipicu sebelum entri arsip dikompresi. |

### setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryCompressed(Event<EntryEventArgsIso> value)
```


Mengatur peristiwa yang dipicu setelah entri arsip telah dikompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | sebuah peristiwa yang dipicu setelah entri arsip telah dikompresi |

