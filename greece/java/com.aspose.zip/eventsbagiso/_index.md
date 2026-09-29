---
title: "EventsBagIso"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Δοχείο συμβάντων που χρησιμοποιείται κατά την αποθήκευση."
type: docs
weight: 66
url: /el/java/com.aspose.zip/eventsbagiso/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagIso
```

Κοντέινερ συμβάντων που χρησιμοποιείται στην αποθήκευση του [IsoArchive](../../com.aspose.zip/isoarchive).
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [EventsBagIso()](#EventsBagIso--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Λαμβάνει ένα συμβάν που ενεργοποιείται πριν μια καταχώρηση αρχείου συμπιεστεί. |
| [getEntryCompressed()](#getEntryCompressed--) | Λαμβάνει ένα συμβάν που ενεργοποιείται μετά τη συμπίεση μιας καταχώρησης αρχείου. |
| [setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Ορίζει ένα συμβάν που ενεργοποιείται πριν μια καταχώρηση αρχείου συμπιεστεί. |
| [setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | Ορίζει ένα συμβάν που ενεργοποιείται μετά τη συμπίεση μιας καταχώρησης αρχείου. |
### EventsBagIso() {#EventsBagIso--}
```
public EventsBagIso()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsIso> getEntryAccessed()
```


Λαμβάνει ένα συμβάν που ενεργοποιείται πριν μια καταχώρηση αρχείου συμπιεστεί.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<EntryEventArgsIso> getEntryCompressed()
```


Λαμβάνει ένα συμβάν που ενεργοποιείται μετά τη συμπίεση μιας καταχώρησης αρχείου.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryAccessed(Event<EntryEventArgsIso> value)
```


Ορίζει ένα συμβάν που ενεργοποιείται πριν μια καταχώρηση αρχείου συμπιεστεί.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | ένα συμβάν που ενεργοποιείται πριν συμπιεστεί μια καταχώρηση αρχείου. |

### setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryCompressed(Event<EntryEventArgsIso> value)
```


Ορίζει ένα συμβάν που ενεργοποιείται μετά τη συμπίεση μιας καταχώρησης αρχείου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | ένα συμβάν που ενεργοποιείται μετά τη συμπίεση μιας καταχώρησης αρχείου |

