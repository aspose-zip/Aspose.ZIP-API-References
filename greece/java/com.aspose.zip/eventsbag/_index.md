---
title: "EventsBag"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Δοχείο συμβάντων που χρησιμοποιείται κατά την αποθήκευση."
type: docs
weight: 65
url: /el/java/com.aspose.zip/eventsbag/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBag
```

Κοντέινερ συμβάντων που χρησιμοποιείται κατά την αποθήκευση του [Archive](../../com.aspose.zip/archive).
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [EventsBag()](#EventsBag--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | Λαμβάνει ένα συμβάν που ενεργοποιείται πριν μια καταχώρηση αρχείου συμπιεστεί. |
| [getEntryCompressed()](#getEntryCompressed--) | Λαμβάνει ένα συμβάν που ενεργοποιείται μετά τη συμπίεση μιας καταχώρησης αρχείου. |
| [setEntryAccessed(Event&lt;EntryEventArgs&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | Ορίζει ένα συμβάν που ενεργοποιείται πριν μια καταχώρηση αρχείου συμπιεστεί. |
| [setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--) | Ορίζει ένα συμβάν που ενεργοποιείται μετά τη συμπίεση μιας καταχώρησης αρχείου. |
### EventsBag() {#EventsBag--}
```
public EventsBag()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgs> getEntryAccessed()
```


Λαμβάνει ένα συμβάν που ενεργοποιείται πριν μια καταχώρηση αρχείου συμπιεστεί.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgs> getEntryCompressed()
```


Λαμβάνει ένα συμβάν που ενεργοποιείται μετά τη συμπίεση μιας καταχώρησης αρχείου.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgs&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public void setEntryAccessed(Event<EntryEventArgs> value)
```


Ορίζει ένα συμβάν που ενεργοποιείται πριν μια καταχώρηση αρχείου συμπιεστεί.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgs&gt; | ένα συμβάν που ενεργοποιείται πριν συμπιεστεί μια καταχώρηση αρχείου. |

### setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--}
```
public void setEntryCompressed(Event<CancelEntryEventArgs> value)
```


Ορίζει ένα συμβάν που ενεργοποιείται μετά τη συμπίεση μιας καταχώρησης αρχείου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgs&gt; | ένα συμβάν που ενεργοποιείται μετά τη συμπίεση μιας καταχώρησης αρχείου |

