---
title: "EventsBagIso"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "सहेजने पर उपयोग किया जाने वाला इवेंट कंटेनर।"
type: docs
weight: 66
url: /hi/java/com.aspose.zip/eventsbagiso/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagIso
```

[IsoArchive](../../com.aspose.zip/isoarchive) को सहेजते समय उपयोग किया जाने वाला इवेंट कंटेनर।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [EventsBagIso()](#EventsBagIso--) |  |
## Methods

| Method | विवरण |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | एक इवेंट प्राप्त करता है जो आर्काइव प्रविष्टि के संपीड़ित होने से पहले उत्पन्न होता है। |
| [getEntryCompressed()](#getEntryCompressed--) | एक इवेंट प्राप्त करता है जो आर्काइव प्रविष्टि के संपीड़ित होने के बाद उत्पन्न होता है। |
| [setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | एक इवेंट सेट करता है जो आर्काइव प्रविष्टि के संपीड़ित होने से पहले उत्पन्न होता है। |
| [setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--) | एक इवेंट सेट करता है जो आर्काइव प्रविष्टि के संपीड़ित होने के बाद उत्पन्न होता है। |
### EventsBagIso() {#EventsBagIso--}
```
public EventsBagIso()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsIso> getEntryAccessed()
```


एक इवेंट प्राप्त करता है जो आर्काइव प्रविष्टि के संपीड़ित होने से पहले उत्पन्न होता है।

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<EntryEventArgsIso> getEntryCompressed()
```


एक इवेंट प्राप्त करता है जो आर्काइव प्रविष्टि के संपीड़ित होने के बाद उत्पन्न होता है।

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryAccessed(Event<EntryEventArgsIso> value)
```


एक इवेंट सेट करता है जो आर्काइव प्रविष्टि के संपीड़ित होने से पहले उत्पन्न होता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | एक इवेंट जो तब उठाया जाता है जब एक आर्काइव एंट्री को संपीड़ित किया जा रहा हो। |

### setEntryCompressed(Event&lt;EntryEventArgsIso&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsIso--}
```
public void setEntryCompressed(Event<EntryEventArgsIso> value)
```


एक इवेंट सेट करता है जो आर्काइव प्रविष्टि के संपीड़ित होने के बाद उत्पन्न होता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsIso&gt; | एक इवेंट जो तब उठाया जाता है जब एक आर्काइव एंट्री संपीड़ित हो चुकी होती है। |

