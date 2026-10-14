---
title: "EventsBagXar"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Δοχείο συμβάντων που χρησιμοποιείται κατά την αποθήκευση."
type: docs
weight: 67
url: /el/java/com.aspose.zip/eventsbagxar/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagXar
```

Δοχείο συμβάντων που χρησιμοποιείται κατά την αποθήκευση του [XarArchive](../../com.aspose.zip/xararchive).
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [EventsBagXar()](#EventsBagXar--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Λαμβάνει ένα συμβάν που ενεργοποιείται πριν μια καταχώρηση αρχείου συμπιεστεί. |
| [getEntryCompressed()](#getEntryCompressed--) | Λαμβάνει ένα συμβάν που ενεργοποιείται μετά τη συμπίεση μιας καταχώρησης αρχείου. |
| [setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--) | Ορίζει ένα συμβάν που ενεργοποιείται πριν μια καταχώρηση αρχείου συμπιεστεί. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--) | Ορίζει ένα συμβάν που ενεργοποιείται μετά τη συμπίεση μιας καταχώρησης αρχείου. |
### EventsBagXar() {#EventsBagXar--}
```
public EventsBagXar()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsXar> getEntryAccessed()
```


Λαμβάνει ένα συμβάν που ενεργοποιείται πριν μια καταχώρηση αρχείου συμπιεστεί.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgsXar> getEntryCompressed()
```


Λαμβάνει ένα συμβάν που ενεργοποιείται μετά τη συμπίεση μιας καταχώρησης αρχείου.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--}
```
public void setEntryAccessed(Event<EntryEventArgsXar> value)
```


Ορίζει ένα συμβάν που ενεργοποιείται πριν μια καταχώρηση αρχείου συμπιεστεί.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsXar&gt; | ένα συμβάν που ενεργοποιείται πριν συμπιεστεί μια καταχώρηση αρχείου. |

### setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--}
```
public void setEntryCompressed(Event<CancelEntryEventArgsXar> value)
```


Ορίζει ένα συμβάν που ενεργοποιείται μετά τη συμπίεση μιας καταχώρησης αρχείου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgsXar&gt; | ένα συμβάν που ενεργοποιείται μετά τη συμπίεση μιας καταχώρησης αρχείου |

